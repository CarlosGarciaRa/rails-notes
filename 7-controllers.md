## CONTROLLERS
After the router has determined which controller to use for a request, the controller is responsible for making sense of the request, and producing the appropriate output.

```
class ArticlesController < ApplicationController
  def index
    articles = Article.all
    render json: serializer.new(articles), status: 200
  end
  def show
    @article = Articles.find(params[:id])
  end

  def serializer
    ArticleSerializer
  end
end
```

## SERIALIZER
After the router has determined which controller to use for a request, the controller is responsible for making sense of the request, and producing the appropriate output.

```
class ArticleSerializer
  include JSONAPI::Serializer
  attributes :title, :content, :slug
end
```


## WRITING REQUESTS RSPEC TESTS
We create `requests` directory under our RSPEC tests directory `spec/request/model_name_spec.rb`

```
# frozen_string_literal: true

require 'rails_helper'

RSpec.describe ArticlesController do
  describe '#index' do
    it 'return a success response' do
      get '/articles'
      expect(response).to have_http_status(:ok)  
    end

    it 'returns a proper JSON' do
      article = create :article
      get '/articles'
      body = JSON.parse(response.body).deep_symbolize_keys
      expect(body).to eq(
        data: [
          {
            id: article.id.to_s,
            type: 'article',
            attributes: {
              title: article.title,
              content: article.content,
              slug: article.slug
            }
          }
        ]
      )
    end
  end
end
```

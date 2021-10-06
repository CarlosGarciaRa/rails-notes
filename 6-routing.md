## ROUTING
We create our route under the directory `config/routes`. Using resources methods gves us al the basic CRUD methods.

```
Rails.application.routes.draw do
  # For details on the DSL available within this file, see https://guides.rubyonrails.org/routing.html
  resources :articles
end


```


## WRITING ROUTE RSPEC TESTS
We create `routing` directory under our RSPEC tests directory `spec/routing/model_name_spec.rb`

```
require 'rails_helper'

RSpec.describe '/articles routes' do
  it 'routes to articles#index' do
    expect(get '/articles').to route_to('articles#index')
  end
end
```

## WRITING CONTROLLER
After the router has determined which controller to use for a request, the controller is responsible for making sense of the request, and producing the appropriate output. We create our controllers under the directory `app/controllers/model_name.rb`

```
class ArticlesController < ApplicationController
  def index
  end
end
```

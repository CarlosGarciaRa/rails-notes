# WRITING TESTS

## WRITING RSPEC TESTS
We create our RSPEC tests under the directory `spec/models/model_name_spec.rb`

```
FactoryBot.define do
  factory :article do
    title { "Sample Article" }
    content { "Sample Content" }
    slug { "sample-article" }
  end
end

```

We can run our test with the command `rspec`, this will output the failing tests. Passing the parameter `--format=documentation` gives us information about all tests.

## WRITING RSPEC TESTS
We create our RSPEC tests under the directory `spec/factories/model_name.rb`

```
RSpec.describe Article, type: :model do
  describe '#validations' do
  let(:article) { FactoryBot.build(:article) }
    it "tests an Article object to be valid" do      
      expect(article).to be_valid
    end
    it "has an invalid title" do
      expect(article).not_to be_valid
      expect(article.errors[:title]).to include("can't be blank")
    end
  end  
end
```

We can run our test with the command `rspec`, this will output the failing tests. Passing the parameter `--format=documentation` gives us information about all tests.

# WRITING RSPEC TESTS
We create our tests under the directory `spec/models/model_name_spec.rb`

```
RSpec.describe Article, type: :model do
  it "tests a number to be positive" do
    expect(1).to be_positive
    expect(5).to be>3
  end
end
```

We can run our test with the command `rspec`, this will output the failing tests. Passing the parameter `--format=documentation` gives us information about all tests.

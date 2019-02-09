# Ruby testing quick commands

## Rspec

### Useful matchers
  ```ruby
  # Change matchers
  expect{Counter.increment}.to change{Counter.count}.from(0).to(1)
  
  
  # Expect message
  allow(obj).to receive(:message).and_return(:value)
  # Compound matcher
  expect(string).to start_with("foo") & end_with("bazz")
  ```

### Stubbing
  ```ruby
  # Stub any instance of a class
  allow_any_instance_of(Class).to receive(:message)
  
  # Double a class
  class_double('Class')
  ```

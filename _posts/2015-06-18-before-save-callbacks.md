---
layout: post
---

## how to test a callback?

i read [this stackoverflow](http://stackoverflow.com/questions/16677718/how-to-test-models-callback-method-independently), but not sure if it applies to before_save callbacks

- you'd have to set the expectation before the object is created, so, you'll run into [expectation set on nil warning](https://relishapp.com/rspec/rspec-mocks/v/2-9/docs/message-expectations/warn-when-expectation-is-set-on-nil#nil-instance-variable)

- you could use `expect_any_instance_of(Object).to receive(:method)` and then create the object

- you can go up a wrench size and assert on whatever the before_save callback does

### references
[rails callbacks](http://api.rubyonrails.org/classes/ActiveRecord/Callbacks.html)

[active record callbacks](http://guides.rubyonrails.org/active_record_callbacks.html)
  - :warning: `update_columns` skips callbacks



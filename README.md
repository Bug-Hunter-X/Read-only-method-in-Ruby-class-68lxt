# Read-only Method Bug in Ruby
This example demonstrates a common error in Ruby where an unintended read-only method is created.  The `value` method is designed for getting the object's value, but it lacks an explicit setter.  Attempts to modify the value using `my_object.value = 20` will fail to change the internal state.

To fix this, you need to explicitly create a setter method.
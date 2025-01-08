# Ruby Instance Variable Modification Bug

This repository demonstrates a potential issue in Ruby when directly manipulating instance variables using `instance_variable_set` or `instance_variable_get`.  This can lead to unexpected behavior and bypasses any intended logic within accessor methods. 

The `bug.rb` file shows how direct manipulation can bypass expected behavior.  The `bugSolution.rb` file demonstrates a more robust approach using accessor methods.

**Key takeaway:**  Favor accessor methods (`attr_accessor`, `attr_reader`, `attr_writer`) for managing instance variable access to ensure code maintainability, readability, and prevent unintended consequences.
# Ruby Bug: Unexpected Behavior When Directly Modifying Instance Variables

This repository demonstrates a common, yet subtle, bug in Ruby related to directly modifying instance variables using `instance_variable_set` and `instance_variable_get`.  Direct manipulation of instance variables can lead to unexpected behavior and make your code difficult to debug and maintain.

The `bug.rb` file shows the problem: modifying the instance variable `@value` directly through `instance_variable_set` circumvents the normal getter and setter methods (if defined), potentially leading to inconsistencies and issues with encapsulation.

The `bugSolution.rb` file provides a solution that employs proper getter and setter methods to ensure controlled access to instance variables, thus enhancing maintainability and predictability.

## How to Run

1. Clone this repository
2. Navigate to the repository's directory.
3. Run `ruby bug.rb` and `ruby bugSolution.rb` to see the output differences.
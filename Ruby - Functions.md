Ruby functions are similar to functions in any other programming language. Ruby Functions are used to bundle one or more repeatable statements into a single unit.

Function names must begin with a lowercase letters. Methods should be defined before calling them, otherwise ruby will raise an exception for undefined method invoking.

```ruby
# Syntax
def function_name
		# expressions....
end

# function with some parameters
def function_name( params ) 
		# expressions....
end

# Calling a Function
def greet(name)
		puts "hello #{name}"
end

function_name("surya")
=> hello surya

# When calling/invoking a function, the braces are optional
function_name "surya"
=> hello surya

# Functions with return statement
def say_hello_to(name)
  return "hello #{name}"
end
puts say_hello_to "dave"
=> "hello dave"

# The return statement is optional, 
# If it's omitted the function will return the last evaluated expression
def get_greeting_for(name)
 "hello #{name}"
end
puts get_greeting_for "dave"
=> "hello dave"

# Default Values
def get_greeting_for(name="anonymous")
  return "hello #{name}"
end
puts get_greeting_for
=> "hello anonymous"
```

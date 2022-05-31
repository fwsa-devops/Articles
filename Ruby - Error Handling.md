# Ruby - Error Handling 

Exception handling is a process which describes a way to handle the error raised in a program. 

Ruby provide a nice mechanism to handle exceptions. We enclose the code that could raise an exception in a begin/end block and use rescue clauses to tell Ruby the types of exceptions we want to handle.

```ruby
# Syntax
begin
		# the expression that we want to execute
rescue TypeError
		# action to take incase of TypeError
rescue ZeroDivisionError
		# action to take incase of ZeroDivisionError	
else
		# action to take incase of any other error
ensure
		# will always be executed 
end
```

```ruby
# Example 1
begin
		number_array = [1,2,3,4,5,6,7]
		puts number_array['a']
rescue
		puts "there was an error"
end

# Example 2
begin
   num 10/0
rescue ZeroDivisionError
  puts "there was an ZeroDivisionError"
ensure
  puts "Ensure always runs"
end
```

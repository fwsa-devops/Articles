# Ruby - Conditional Statement

Ruby offers conditional structures that are pretty common to modern languages. There are various types of if statement in Ruby

- if statement
- if-else statement
- if-else-if statement
- ternary statement
- unless statement
- case statement

### If Statement

```ruby
# Syntax
if condition
		# expressions...
end

# Example
age = gets.chomp.to_i   
if age >= 18   
  puts "You are eligible to vote."   
end
```

### If-else statement

```ruby
# Syntax
if condition
		# conditional match expressions....
else
		# conditional does not match expressions...
end

# Example
age = gets.chomp.to_i   
if age >= 18   
  puts "You are eligible to vote."   
else   
  puts "You are not eligible to vote."   
end
```

### if-else-if statement

```ruby
# Syntax
if condition1
		# expression if condition1 matches
elsif condition2
		# expression if condition2 matches
else
		# expression of no condition matches
end

# Example
x = gets.chomp.to_i
if x > 2
   puts "x is greater than 2"
elsif x <= 2 and x!=0
   puts "x is 1"
else
   puts "Can't guess the number"
end
```

### Ternary statement

```ruby
# Syntax
condition ? if-true-expression : if-false-expression

# Example
random_number = gets.chomp.to_i;   
a = (random_number > 3 ? true : false);    
puts a
```

### Unless statement

**Executes** *code* **if *conditional*** is **false**. If the *conditional*  is true, code specified in the else clause is executed.

```ruby
# Syntax
unless conditional
		code
	else
		code
end

# Example
x = gets.chomp.to_i 
unless x>=2
   puts "x is less than 2"
 else
   puts "x is greater than 2"
end
```

### Case statement

```ruby
# Syntax
case expr0
	when expr1, expr2
		stmt1
	when expr3, expr4
		stmt2
	else
		stmt3
end

# Example
$age =  gets.chomp.to_i
case $age
when 0 .. 2
   puts "baby"
when 3 .. 6
   puts "little child"
when 7 .. 12
   puts "child"
when 13 .. 18
   puts "youth"
else
   puts "adult"
end
```

Ruby shares a neat feature with Perl that is statement modifier, that lets you tack conditional statements onto the end of a normal statement.

- if modifier
- unless modifier

### if modifier

```ruby
# Synatx
code if condition

# Example
$age = gets.chomp.to_i
puts "debug" if $age
```

### Unless modifier
```ruby
# Synatx
code unless condition

# Example
$var =  gets.chomp.to_i
print "1 -- Value is set\n" if $var
print "2 -- Value is set\n" unless $var

$var = false
print "3 -- Value is set\n" unless $var
```

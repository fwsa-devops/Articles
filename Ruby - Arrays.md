# Ruby - Arrays

Ruby arrays are ordered, integer-indexed collections of any object. Each element in an array is associated with and referred to by an index. Array Index starts at 0, similar to Java and C.

Ruby arrays can hold objects such as String, Integer, Fixnum, Hash, Symbol, even other Array objects.

```ruby
# Creating a Array
students = Array.new

# Creating a Array with a fixed length
students = Array.new(10)

# pushing a value inside an array
students[0] = "surya"
students[1] = 10
students[2] = 11.0
students[3] = {name => "surya"}
students[5] = ["a", "b", "c"]

# log of students
puts students
surya
10
11.0
{name => "surya"}

["a","b", "c"]

# Accessing Element inside an array
puts students[0]
surya

# Accessing specific set of Elements inside an array
puts students[1, 3]
passing a second argument gets us all the elements with in the index range 
except the last element
["surya", 10, 11.0]

```

## Built-in Methods

```ruby
# Creating a Array
students = Array.new

# pushing a value inside an array
students[0] = "surya"
students[1] = 10
students[2] = 11.0
students[3] = {name => "surya"}
students[5] = ["a", "b", "c"]

Methods
# .length() methods return the length of the array. 
# .size() method can also be used to get length of an array
students.length()

# .push method appends the element at the end of an array
students.push()

# .pop method Removes the last element and returns it, or nil if the array is empty
students.pop()

# .index method returns the **index of first matching element**. 
# If no match found method return **nil**
students.index()

# .include? Returns **true** if the given object is present, otherwise returns false.
students.include?("surya")

# .sort() methods helps us sort the element is Asc or Desc order.
# This only works if all the elements inside the array are of the same datatype
students.sort()

# .reverse Returns a new array containing the same elements in reverse order.
students.reverse()
```

[]()

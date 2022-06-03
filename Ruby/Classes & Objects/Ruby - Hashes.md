# Ruby - Hashes

A Hash is a collection of key-value pairs like this: `"name" = > "surya"`. It is similar to an Array, except that indexing is done via arbitrary keys of any object type, not an integer index.

The default value of an hash is `nil`

```ruby
# Creating a Hash
students = Hash.new
students = { "name" => "surya", "team" => "CSR", 1 => "some number"  }

# replacing the default nil with custom value
students = Hash.new("foo")
puts "#{students[0]}" 
puts "#{students[99]}"

Output:
foo
foo

# passing some key-value inside hash
# students[key] = value
students["name"] = "surya"
```

Built-in Methods

```ruby
# .clear method Removes all hash entries and returns self.
students.clear()

# .compact method returns a new copy with all the nil-valued entries removed
students = { 1 => "foo" ,  2=> nil, 3=> nil , "name" => "surya"  }
puts students.compact
{ 1=> foo, "name" => "surya" }

# .compact! method returns self with all the nil-valued entries removed
# returns nil if no entries were removed
students = { 1 => "foo" ,  2=> nil, 3=> nil , "name" => "surya"  }
puts students.compact!
{ 1=> foo, "name" => "surya" }

```

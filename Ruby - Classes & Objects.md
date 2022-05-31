# Ruby - Classes & Objects

In object-oriented programming, a **class** is a blueprint for creating **objects** (a particular data structure), or a class is a template definition of the methods and variables in a particular kind of object . Thus, an object is a specific instance of a class; it contains real values instead of variables

Ruby is a perfect Object Oriented Programming Language. The features of the object-oriented programming language include −

- Data Encapsulation
- Data Abstraction
- Polymorphism
- Inheritance

```ruby
# Syntax
class Book

		# Constructor
		def initialize
				# expressions....
		end
end

# Example
class Book 
		@title
		@author
		@page

		def initialize(title, author, page)
				@title = title
				@author = author
				@page = page
		end

		def get_title
				@title
		end

		def set_title (title)
				@title = title
		end

		def get_author
				@author
		end

		def set_author (author)
				@author = author
		end

		def get_page
				@page
		end

		def set_page (page)
				@page = page
		end

end
```

## Attribute in Ruby

In OOP, the `member access control` concept is important as it allows to control the access to encapsulated variables. 

In many programming languages, this concept is implemented by using `getters` and `setters` for each member.

In Ruby, the `attr_*` methods are in charge of the `member access control`.

- `attr` method
- `attr_reader` method
- `attr_writer` method
- `attr_accessor` method

### attr

The `attr` method creates an instance variable and a **getter** method for each attribute name passed as argument

An argument can be a `Symbol` or a `String` that will be converted to `Symbol`

```ruby
class Attr
	attr :attr1, 'attr2'
end

irb> Attr.instance_methods
 => [:attr1, :attr2]
```

### attr_reader

the `attr_reader` method is similar to `attr`

```ruby
class Attr
	attr :attr1, 'attr2'
end

irb> Attr.instance_methods
 => [:attr1, :attr2]
```

### attr_writer

the `attr_writer` method creates an instance variable and a **setter** method for each attribute name passed as argument

An argument can be a `Symbol` or a `String` that will be converted to `Symbol`

```ruby
class Attr
	attr :attr1, 'attr2'
end

irb> Attr.instance_methods
 => [:attr1=, :attr2=]
```

### attr_accessor

the `attr_accessor` method creates an instance variable, a getter and a setter method for each attribute name passed as argument

An argument can be a `Symbol` or a `String` that will be converted to `Symbol`

```ruby
module Attr
  attr_accessor :attr1, 'attr2'
end

irb> Attr.instance_methods.sort
 => [:attr1, :attr1=, :attr2, :attr2=]
```

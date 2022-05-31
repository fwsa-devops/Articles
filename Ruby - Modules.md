# Ruby - Modules

A module is a collection of methods, variables and constants stored in a container.It is similar to a class but it cannot be instantiated. The name a module must begin with a Uppercase.

```ruby
# Example
# the module keyword is used to define a new module
module Tool
		def say_hi
			puts "Hi sir"
		end

		def say_bye
			puts "Bye sir"
		end
end
```

Modules have 2 main purposes:

- providing a namespace and prevent name clashes
- using the mixin facility for composition

## Module as namespace

Namespaccing is  a way of bundling logically related object together. Modules allows classes or modules with conflicting names to co-exist while avoiding collisions.

```ruby
# tools.rb
module Tools
  class Array
      # ...
      def hello
          puts "hello Array"
      end

  end
end
```

Here we can see that the `Array` class is defined within the scope of the `Tools` module. To access this class from outside of the module `Rails`, we use the `::` syntax.

```ruby
# another ruby file
require_relative "variables.rb"

include Tools

array = Tools::Array.new
puts array.hello

=> hello Array
```

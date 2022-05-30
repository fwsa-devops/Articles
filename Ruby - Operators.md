# Ruby - Operators

An operator is **a symbol that represents an operation to be performed with one or more operand.** Operators are the foundation of any programming language. Ruby supported operators are:

- Arithmetic Operator
- Bitwise Operator
- Comparison Operator
- Unary Operator
- Logical Operator
- Ternary Operator
- Range Operator
- Assignment Operator

## Arithmetic Operator

These are used to perform arithmetic/mathematical operations on operand. 

+ - Add Values from both the sides of the operator.

- - Subtract values from both sides of the operator. 

/ - Divide left side operand with right side operand.

* - Multiply values from both sides of the operator.

** - Right side operand becomes the exponent of left side operand.

% - Divide left side operand with right side operand returning remainder.

## Bitwise Operator

Bitwise operators **work directly on the binary representations of integers in memory**.

& - AND operator

|- OR operator

<< - Left shift operator

>> - Right Shift operator

^ - XOR operator

~ - Complement operator

## Comparison Operator

Comparison operator takes simple values as arguments and used to check for equality between two values.

== - Equal operator

!= - Not Equal operator

> - Left operand is greater than right operand

< - Right operand is greater than left operand

>= - Left operand is greater than or equal to right operand

<= - Right operand is greated than or equal to left operand

<=> - Combined Comparison operator

.eql? - checks for equality and type of the operands

equal? - Checks for the object ID

## Unary Operator

Unary operator takes a single value as argument and operates on that.

! - Boolean Not

~ - Bitwise complement

+ - Unary plus

## Logical Operator

&& or “and” - AND operator, If both the operands are true, then the condition becomes true  

|| or “or” - OR operator, If any of the operands is true, then the condition becomes true 

! or “not” - NOT operator, Used to reverses the logical state of its operand.

## Ternary Operator

There is one more operator called Ternary Operator. It first evaluates an expression for a true or false value and then executes one of the two given statements depending upon the result of the evaluation

?: - Conditional Expression

```ruby
if condition ? true_part : false_part
```

## Range Operator

Range Operator is used to create a range of successive values - consisting of a start value, an end value, and a range of values in between.

The (..) creates a range including the last term. `1..5` ⇒ 1 to 5

The (...) creates a range excluding the last term. `1...5` ⇒ 1 to 4

## Assignment Operator

Assignment Operator is used to assign a value to the operand

= - Simple Assignment operator

+=  - Add Assignment operator

-=  - subtract Assigment operator

*=  - Multiply Assignment operator

/=  - Divide Assignment operator

%=  - Modulus Assignment operator

**=  - Exponential Assignment operator

# Javascript Operators

JavaScript includes operators as in other languages. An operator performs some operation on single or multiple operands (data value) and produces a result. For example 1 + 2, where + sign is an operator and 1 is left operand and 2 is right operand. + operator adds two numeric values and produces a result which is 3 in this case.
JavaScript includes operators as in other languages. An operator performs some operation on single or multiple operands (data value) and produces a result. For example 1 + 2, where + sign is an operator and 1 is left operand and 2 is right operand. + operator adds two numeric values and produces a result which is 3 in this case.

JavaScript includes following categories of operators. 

1.	Arithmetic Operators 
2.	Comparison Operators 
3.	Logical Operators 
4.	Assignment Operators 
5.	Conditional Operators 

# Arithmetic Operators

Arithmetic operators are used to perform mathematical operations between numeric operands. 
![]( https://www.devopsschool.com/blog/wp-content/uploads/2020/07/JavaScript-Arithmatic-Operators.png)
Example: + operator
var a = 5, b = "Hello ", c = "World!", d = 10;

a + b; // "5Hello "

b + c; // "Hello World!"

a + d; // 15
# Comparison Operators
JavaScript language includes operators that compare two operands and return Boolean value true or false. 
![]( https://www.oreilly.com/library/view/visual-basic-2012/9781118332085/images/f253-01.jpg)

Example: Comparison Operators 

var a = 5, b = 10, c = "5";
var x = a;

a == c; // returns true

a === c; // returns false

a == x; // returns true

a != b; // returns true

a > b; // returns false

a < b; // returns true

a >= b; // returns false

a <= b; // returns true

a >= c; // returns true

a <= c; // returns true

# Logical Operators

Logical operators are used to combine two or more conditions. JavaScript includes following logical operators. 

![]( https://programmingwithbabu.files.wordpress.com/2017/09/logical_operator_in_c.jpg)

Example: Logical Operators 
var a = 5, b = 10;

(a != b) && (a < b); // returns true

(a > b) || (a == b); // returns false

(a < b) || (a == b); // returns true

!(a < b); // returns false

!(a > b); // returns true


# Assignment Operators
JavaScript includes assignment operators to assign values to variables with less key strokes. 
Example: Assignment operators 
var x = 5, y = 10, z = 15;

x = y; //x would be 10

x += 1; //x would be 6

x -= 1; //x would be 4

x *= 5; //x would be 25

x /= 5; //x would be 1

x %= 2; //x would be 1

# Expressions
Expressions perform operations on data and move data around. Some expressions will be evaluated for their results, some for their side effects, some for both. An expression can have three kinds of result: 
1.	a value, such as the result of: (4 * i) 
2.	a variable, such as the result of: i = 4 
3.	nothing (in the case of an invocation of a method declared as void) 
An expression that results in a variable is called an lvalue in C++ and many other languages. A variable expression in Java is the same thing, the Java Language Specification just uses the name variable instead of lvalue. Such an expression can be used on the left hand side of an assignment operator. Side effects come about when an expression includes an assignment, increment, decrement, or method invocation.

# Functions

Functions are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. To use a function, you must define it somewhere in the scope from which you wish to call it.


> by kefah
# Comparison and Logical Operators

![ggg](https://chunxuchai.files.wordpress.com/2019/05/comparison-operator.jpg)

The field of computer science has many foundations in mathematical logic. If you have a familiarity with logic, you know that it involves truth tables, Boolean algebra, and comparisons to determine equality or difference.
The JavaScript programming language uses operators to evaluate statements that can aid in control flow within programming. 
In this tutorial, we’ll go over logical operators. These are commonly used with conditional statements, and the if, else, and else if keywords, as well as the ternary operator. If you are interested in learning more about conditional statements first, refer to How To Write Conditional Statements in JavaScript.
Comparison Operators
In JavaScript, there are a number of comparison operators that you can use to evaluate whether given values are different or equal, as well as if a value is greater than or less than another. Often, these operators are used with stored values in variables. 
Comparison operators all return a Boolean (logical) value of true or false. 
The table below summarizes the comparison operators available in JavaScript.
Operator	What it means
==	Equal to
!=	Not equal to
===	Strictly equal to with no type conversion
! ==	Strictly unequal to with no type conversion
>	Greater than
>=	Greater than or equal to
<	Less than
<=	Less than or equal to
Let’s go into each operator in detail. 
Equality
The equality operator measures whether values on either side of the operator are equal.
Let’s consider the following:
let x = 3;

x == 3;
 
Because 3 is equivalent to 3, the output received will be the Boolean value of true.
Output
true
If we instead test whether x is equal to another integer, we’ll receive output stating that the statement is validated to be false. 
let x = 3;

x == 5;
 
Output
false
With this equivalency expression, you can also test other data types such as strings and Booleans. 
We’ll use a string example below.
let shark = 'sammy';

shark == 'sammy';
shark == 'taylor';
 
Output
true
false
In the first instance, the expression returned true because the strings were equivalent. In the second instance, of shark == 'taylor', the expression returned false because the strings were not equal.
Worth noting, is that the == operator is not a strict equivalency, so you can mix numbers and strings that evaluate to being equivalent. Consider the following example.
let x = 3;

x == '3';
 
Even though the first line uses a number data type, and the second line tests x against a string data type, both values equal 3, and the output you will receive indicates that the expression is true.
Output
true
Because this operator is not strict about data type, it can support users entering strings instead of numbers, for example. There is no need to convert data types to test equivalency. 
There are many cases where you may use comparison operators like the == operator. You may want to test equivalency when grading a test, for example. That way you can validate whether a given answer is correct or not.
let answer = 10;
let response = prompt("What is 5 + 5?");

if (answer == response) {
  console.log("You're correct!");
}
 
Here, if the student enters 10 in response to the question when prompted, they will receive the feedback that they are correct. 
There are many potential applications of comparison operators in JavaScript, and they will help you control the flow of your program. 
Now that you have a foundation with a few examples for ==, we’ll be a bit briefer going forward.
Inequality
The != operator tests inequality, to determine whether the values on either side of the operator are not equal.
Let’s consider an example.
let y = 8;

y != 9;
 
For this example, 8 does not equal 9, so the expression will be evaluated to be true:
Output
true
For a statement of inequality to be considered false, the two values on either side would need to actually be equal, as in the following.
let y = 8;

y != 8
 
Output
false
In this second example, the two values on either side of the operator are equal, so the expression is not true.
Identity
The === operator determines whether two values are both of equal value and of equal type. This is also known as a strict equality operator. This means you cannot mix number and string data types.
Here’s an example:
let z = 4;

z === 4;

z === '4';
 
We’ll receive the following output.
Output
true

false
The example indicates that z is strictly equal to 4 (as it is assigned the numeric value of 4), but that it is not strictly equal to the string '4'.
Because this operator is strict, you will need to keep in mind that you may need to convert user-entered data from one data type to another, for instance, when working with the identity operator. This may help you keep data types consistent throughout your program.
Non Identity
Like ===, the operator !== evaluates a strict inequality, which considers both the value and the type of the operands on either side of the operator.
We’ll review the following examples.
let a = 18;

a !== 18;

a !== '18';

a !== 29;
 
The output for the above will be as follows.
Output
false 

true

true
In this example, since a does strictly equal 18, the first expression evaluates to false as we are testing inequality. In the next two examples, a is determined to be unequal to the string '18' and the number 29, so those two expressions evaluate to true (since they are not equal). 
Greater than
The greater than symbol in JavaScript may be familiar to you from math: >. This evaluates whether one value (on the left side of the expression) is greater than another value (on the right side of the expression). 
Like the == operator above, the greater than operator is not strict, and therefore will allow you to mix strings and numbers.
Let’s consider the following examples.
let f = 72;

f > 80;

f > '30';
 
We’ll receive the following output:
Output
false

true
In the first instance, 72 is less than 80, so the first expression evaluates to false. In the second instance, 72 is in fact greater than '30', and the operator does not care that the number is a string, so the expression evaluates to true.
Greater than or equal
Similarly, the operator for greater than or equal to will evaluate whether one operand meets the threshold of the other. This operator is typed as >= a kind of compound between greater than (>) and the equal sign (=). 
Our examples:
let g = 102;

g >= 90;

g >= 103;
 
Output
true

false
Because 102 is a larger number than 90, it is considered to be greater than or equal to 90. Because 102 is less than 103, it is false to state that 102 >= 103. If either 90 or 103 were a string data type, the expressions would also evaluate the same. 
Less than
The less than operator appears as the mirror version of the greater than operator: <. 
Consider the following examples as a demonstration.
let w = 1066;

w < 476;

w < 1945;
 
Output
false

true
Here, 1066 is greater than 476, so the expression evaluates to false. However, 1066 is less than 1945, so the second statement evaluates to true. Again, the 476 or 1945 values could also be strings. 
Less than or equal
The opposite of greater than or equal, the less than or equal operator — <= — will evaluate whether the value on the left side of the operator is less than or equal to the value on the right side.
Here are a few examples.
let p = 2001;

p <= 1968;

p <= 2001;

p <= 2020;
 
Output
false

true

true
The first expression evaluates to false because 2001 is not less than or equal to 1968. In the second expression, because the variable and 2001 are equal values, the output is true. In the third expression, the output is also true because 2001 is less than 2020. Again, these values could also be represented as strings, as in '2001', and would evaluate in the same manner.
Note: Be sure not to confuse the less than or equal operator (<=) with the arrow function (=>) in JavaScript. Learn more about arrow functions in our tutorial Understanding Arrow Functions in JavaScript. 
To understand how these comparison operators can work together in a program, refer to our grades.js example in our How To Write Conditional Statements in JavaScript tutorial. 
Logical Operators
In JavaScript, there are three logical operators, which connect two or more programming statements to return a true (also called “truthy”) or false (“falsy”) value. These are most often used with Boolean (logical) types, but can be applied to values of any data type. 
These logical operators are summarized in the table below.
Operator	Syntax	Description
AND	&&	Returns true if both operands are true
OR	||	Returns true if either operand is true
NOT	!	Returns true if operand is false
Let’s review each of these operators in more detail.
AND
The AND operator is represented by two ampersands — && — it will return true if the operands to the left and right evaluate to be true. 
For example, with AND we can check if something is both high quality and has a low price.
// High quality and low price are true
const highQuality = true;
const lowPrice = true;

(highQuality && lowPrice);
 
Output
true
Since both variables evaluate to be true, the AND operation within the parentheses returns true. If either one of the variables were initialized as false, the && expression would evaluate to false. 
OR
The OR operator is represented by two pipes — || — it will return true if one of the operands is true. 
In this example, we’ll check if something is either highQuality or lowPrice.
// Only low price is true
const highQuality = false;
const lowPrice = true;

(highQuality || lowPrice);
 
Output
true
Since one of the two conditions (highQuality or lowPrice) was true, the whole operation returns true. This would only evaluate to false if both conditions were false.
NOT
The NOT operator is represented by an exclamation point — ! — it will return true if the operand is set to false, and vice versa.
const highQuality = true;

!(highQuality);
 
Output
false
In the above statement, highQuality has the value of true. With the NOT operator, we are checking to see if hiqhQuality evaluates to false. If it were false, the output would return true, but since it is true, the output returns false.
The NOT operator is a bit tricky to understand at first. The important part to remember is that NOT checks whether something evaluates to be false.
Conclusion
Logical operators are the building blocks of flow control in JavaScript programming. Using these operators effectively will help you develop programs that evaluate statements and move to the next stage based on whether a statement is true or false. 
To continue learning more about JavaScript, check out our How To Code in JavaScript series, and our JavaScript tag. 




# JavaScript while Loop and For Loop
![ggg](https://cdn.programiz.com/sites/tutorial2program/files/javascript-while-loop.png)


The while statement creates a loop that executes a specified statement as long as the test condition evaluates to true. The condition is evaluated before executing the statement
JavaScript while Loop
The syntax of the while loop is:
while (condition) {
    // body of loop
}
Here,
1.	A while loop evaluates the condition inside the parenthesis ().
2.	If the condition evaluates to true, the code inside the while loop is executed.
3.	The condition is evaluated again.
4.	This process continues until the condition is false.
5.	When the condition evaluates to false, the loop stops.
JavaScript Loops

# The while Loop
This is the simplest looping statement provided by JavaScript.
The while loop loops through a block of code as long as the specified condition evaluates to true. As soon as the condition fails, the loop is stopped. The generic syntax of the while loop is:
while(condition) {
    // Code to be executed
} 
The following example defines a loop that will continue to run as long as the variable i is less than or equal to 5. The variable i will increase by 1 each time the loop runs:
Example
Try this code »
var i = 1;
while(i <= 5) {    
    document.write("<p>The number is " + i + "</p>");
    i++;
}
Note: Make sure that the condition specified in your loop eventually goes false. Otherwise, the loop will never stop iterating which is known as infinite loop. A common mistake is to forget to increment the counter variable (variable i in our case). 

# The for Loop

The for loop repeats a block of code as long as a certain condition is met. It is typically used to execute a block of code for certain number of times. Its syntax is:
for(initialization; condition; increment) {
    // Code to be executed
} 
The parameters of the for loop statement have following meanings:
•	initialization — it is used to initialize the counter variables, and evaluated once unconditionally before the first execution of the body of the loop.
•	condition — it is evaluated at the beginning of each iteration. If it evaluates to true, the loop statements execute. If it evaluates to false, the execution of the loop ends.
•	increment — it updates the loop counter with a new value each time the loop runs.
The following example defines a loop that starts with i=1. The loop will continued until the value of variable i is less than or equal to 5. The variable i will increase by 1 each time the loop runs:
Example
Try this code »
for(var i=1; i<=5; i++) {
    document.write("<p>The number is " + i + "</p>");
}
The for loop is particularly useful for iterating over an array. The following example will show you how to print each item or element of the JavaScript array.
Example
Try this code »
// An array with some elements
var fruits = ["Apple", "Banana", "Mango", "Orange", "Papaya"];
 
// Loop through all the elements in the array 
for(var i=0; i<fruits.length; i++) {
    document.write("<p>" + fruits[i] + "</p>");
}


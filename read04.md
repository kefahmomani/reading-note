#  what is the javascrept


![ggg](https://miro.medium.com/max/700/1*JTVWHBtzlA9P6iKMxCF2yQ.png)

JavaScript is one of the most popular programming languages in the world.
Can be use for the most web application such  as 
•	websites
•	web applications
•	server-side applications using Node.js
JavaScript is a programming language that is:
•	high level: it provides abstractions that allow you to ignore the details of the machine where it's running on. It manages memory automatically with a garbage collector, so you can focus on the code instead of managing memory like other languages like C would need, and provides many constructs which allow you to deal with highly powerful variables and objects.
•	dynamic: opposed to static programming languages, a dynamic language executes at runtime many of the things that a static language does at compile time. This has pros and cons, and it gives us powerful features like dynamic typing, late binding, reflection, functional programming, object runtime alteration, closures and much more. Don't worry if those things are unknown to you - you'll know all of them by the end of the course.
•	dynamically typed: a variable does not enforce a type. You can reassign any type to a variable, for example, assigning an integer to a variable that holds a string.
•	loosely typed: as opposed to strong typing, loosely (or weakly) typed languages do not enforce the type of an object, allowing more flexibility but denying us type safety and type checking (something that TypeScript - which builds on top of JavaScript - provides)
•	interpreted: it's commonly known as an interpreted language, which means that it does not need a compilation stage before a program can run, as opposed to C, Java or Go for example. In practice, browsers do compile JavaScript before executing it, for performance reasons, but this is transparent to you - there is no additional step involved.
•	multi-paradigm: the language does not enforce any particular programming paradigm, unlike Java for example, which forces the use of object-oriented programming, or C that forces imperative programming. You can write JavaScript using an object-oriented paradigm, using prototypes and the new (as of ES6) classes syntax. You can write JavaScript in a functional programming style, with its first-class functions, or even in an imperative style (C-like).
In case you're wondering, JavaScript has nothing to do with Java, it's a poor name choice but we have to live with it.


# A brief intro to the syntax of JavaScript


![ggg](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2018/01/Java-Syntax.jpg)
In this little introduction I want to tell you about 5 concepts:
•	white space
•	case sensitivity
•	literals
•	identifiers
•	comments
## White space
JavaScript does not consider white space meaningful. Spaces and line breaks can be added in any fashion you might like, at least in theory.
In practice, you will most likely keep a well defined style and adhere to what people commonly use, and enforce this using a linter or a style tool such as Prettier.
For example, I always use 2 space characters for each indentation.
##  Case sensitive
JavaScript is case sensitive. A variable named something is different than Something.
The same goes for any identifier.
##  Literals
We define literal as a value that is written in the source code, for example, a number, a string, a boolean or also more advanced constructs, like Object Literals or Array Literals:
5
'Test'
true
['a', 'b']
{color: 'red', shape: 'Rectangle'}
## Identifiers
An identifier is a sequence of characters that can be used to identify a variable, a function, or an object. It can start with a letter, the dollar sign $ or an underscore _, and it can contain digits. Using Unicode, a letter can be any allowed character, for example, an emoji ?.
Test
test
TEST
_test
Test1
$test
The dollar sign is commonly used to reference DOM elements.
Some names are reserved for JavaScript internal use, and we can't use them as identifiers.
## Comments
Comments are one of the most important parts of any program, in any programming language. They are important because they let us annotate the code and add important information that otherwise would not be available to other people (or ourselves) reading the code.
In JavaScript, we can write a comment on a single line using //. Everything after // is not considered as code by the JavaScript interpreter.
Like this:
// a comment
true //another comment
Another type of comment is a multi-line comment. It starts with /* and ends with */.
Everything in between is not considered as code:
/* some kind
of 
comment 

*/


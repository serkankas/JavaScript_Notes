## Core JavaScript Language

This markdown will contain course content for JavaScript programming. Consider that I am totally beginner for JavaScript language. Some of my examples/syntaxing/logic may not fully correct. I will fix it as soon as I learn the better way.<br>
With that being said, let's dive into learning JavaScript. Here's the [link](https://www.youtube.com/watch?v=PkZNo7MFNFg) that I follow as main course. Feel free to check it by yourself. 

<hr>

Topics:

1. [Running JavaScript](#chapter1)
1. [Comments](#chapter2)
1. [Data Types](#chapter3)
1. [Assignment Operator](#chapter4)
1. [Case Sensitivity](#chapter5)

<hr>

<section id="chapter1"></section>

> Running JavaScript

You do not need to install JavaScript to run it initially. Because, most of the current used website already support the JavaScript by its own.<br>
The Tutorial has some suggestion however, I plan to use this [link](https://playcode.io/javascript) to follow along. You can change your preference for your application.

<section id="chapter2"></section>

> Comments

Usage of comment is, letting other user what's your comment about that line/function/variable, etc. Commenting your own code will help you and people who will look at your written code to clearify most of the work if not obvious. In JavaScript, comment syntax is similar to C language.

```js
// This is comment for single line

/*
This is
Comment
For
Multiple
Line
*/
```

As the usage clearify, comments are the lines that doesn't compile as program but it will be ignored from the compiler, program, etc.

<section id="chapter3"></section>

> Data Types

Data types is a variety of things that computer can understand, compute and decide based on values.

JavaScript provide 7 mandatory data-type.

1. Undifined
1. Null
1. Boolean
1. String
1. Symbol
1. Number
1. Object

In order to store data type in some memory location in program, we have to use variable. ~~Like in other programming language, etc.~~

```js
var myName = "Serkan K"
let phrase = "This is not a Game!"
const pi = 3.141592

myName = 12
```

There are three different variable decleration in JavaScript.

|Keyword| Usage Case
|---|---
|var| Can be used in anywhere in program
|let| Can be used inside the scope where you declare. Cannot be used outside of scope.
| const | Constant, cannot be changed. Unlike var and let.

<section id="chapter4"></section>

> Assignment Operator

There is a difference between declaration and assignment for variable. What is the difference you may ask. Assignment is set a variable with a variable-name without declare any type for it. Where as decleration, is setting/assigning variable with corresponded data type declaring with it. Honestly, I do not focus on that the topic that much since, you get used to use as you wish, doesn't matter what is what at the end of the day. If you wish, you can read the [article](https://makersaid.com/declare-vs-assign-in-javascript/#:~:text=The%20Difference%20Between%20Declaring%20and,to%20give%20it%20a%20value.) about it.

```js
var assignment;         // Declaration
var declaration = 5;    // Declaration & Assignment

declaration = 10;       // Assignment
```

You may realize that I do use semicolon to end line. This is __NOT__ required but recommended way to end the line.

Before we end this session, I will give function that will act like print function for other programming language. Which is ```console.log();```. This is function that we use for debugging purpose printing screen. It will be used alot in this series.

```js
console.log("This is a text");

var a = "Other text";

console.log(a);
```

<section id="chapter5"></section>

> Case Sensitivity

JavaScript, like most of the programming language, is case sensitive for function/variable names.

For the people who don't know what that mean is, that means ```variableName != VariAbleName```. I do suggest that pick one or two different variable naming style and keep following that structure for your whole project. It will make your code easy to follow and make more readable. Here is a [link](https://www.theserverside.com/feature/A-guide-to-common-variable-naming-conventions) that you can check for conventional ones.

<section id="chapter6"></section>

> Arithmetic Operators

| Symbol | Application
| -- | --
| + | Addition
| - | Subtraction
| * | Multiplication
| / | Division
| % | Modulus (Reminder)
| ** | Exponentiation
| ++ | Increment
| -- | Decrement 
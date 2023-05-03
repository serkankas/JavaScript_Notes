## Core JavaScript Language

This markdown will contain course content for JavaScript programming. Consider that I am totally beginner for JavaScript language. Some of my examples/syntaxing/logic may not fully correct. I will fix it as soon as I learn the better way.<br>
With that being said, let's dive into learning JavaScript. Here's the [link](https://www.youtube.com/watch?v=PkZNo7MFNFg) that I follow as main course. Feel free to check it by yourself. 

Topics:

1. [Running JavaScript](#chapter1)
1. [Comments](#chapter2)
1. [Data Types](#chapter3)

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


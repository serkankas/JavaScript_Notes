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
1. [Arithmetic Operator](#chapter6)
1. [Logical Operator](#chapter7)
1. [Shift & Bitwise Operators](#chapter8)
1. [Arithmetic Assignment Operators](#chapter9)
1. [Shift Assignment Operators](#chapter10)
1. [Bitwise Assignment Operators](#chapter11)
1. [Logical Assignment Operators](#chapter12)
1. [Escape Character](#chapter13)
1. [String Identification](#chapter14)
1. [String Operations](#chapter15)
1. [Array Declaration](#chapter16)
1. [Nested Arrays](#chapter17)
1. [Accessing Array Element and Manipulating](#chapter18)
1. [Manipulating Arrays with Push, Pop, Shift and Unshift Functions](#chapter19)
1. [Creating own functions](#chapter20)
1. [Local and Global scopes for variables.](#chapter21)

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

<section id="chapter7"></section>

> Logical Operators

| Symbol | Application
| -- | --
| == | Equal to
| === | Equal to & same type checker
| != | Not equal to
| !== | Not equal to | Not same type checker
| > | Greater than
| < | Less than
| >= | Greater than or equal to
| <= | Less than or equal to

<section id="chapter8"></section>

> Shift & Bitwise Operators

| Operator | Name | Description
| -- | -- | --
| & | AND | Set result to one if both bits are 1
| \| | OR | Set result to one if any of the bit is 1
| ^ | XOR | Set result to one if one of two bit is 1
| ~ | NOT | Invert the bit
| >> | Left Shift | Shift left by pushing zero from the right, going to lose leftmost bits.
| << | Right Shift | Shift right by pushing zero from left, going to lose rightmost bits.
| >>> | Right shift without sign | __I do not clearly understand what it does, may be check and fixed it later!__

I believe the example in [link](https://www.w3schools.com/js/js_bitwise.asp) is a bit clearer.

```js
// Example in 32 bit.

// 5            00000000 00000000 00000000 00000101
// 5 >> 1       00000000 00000000 00000000 00000010 (2)
// 5 >>> 1      00000000 00000000 00000000 00000010 (2)

// -5           11111111 11111111 11111111 11111011
// -5 >> 1      11111111 11111111 11111111 11111101 (-3)
// -5 >>> 1     01111111 11111111 11111111 11111101 (2147483645)
// -5 >>> 2     00111111 11111111 11111111 11111110 (1073741822)
```

So __>>>__ is still right shift, but it behave different for unsigned numbers. Usage is different in negative integer values.

<section id="chapter9"></section>

> Arithmetic Assignment Operators

| Operator | Example Usage | Meaning of
| -- | -- | --
| = | x = y | x = y
| += | x += y | x = x + y
| -= | x -= y | x = x - y
| *= | x *= y | x = x * y
| /= | x /= y | x = x / y
| %= | x %= y | x = x % y
| **= | x **= y | x = x ** y

<section id="chapter10"></section>

> Shift Assignment Operators

| Operator | Example Usage | Meaning of
| -- | -- | --
| <<= | x <<= y | x = x << y
| >>= | x >>= y | x = x >> y
| >>>= | x >>>= y | x = x >>> y

<section id="chapter11"></section>

> Bitwise Assigment Operators

| Operator | Example Usage | Meaning of
| -- | -- | --
| &= | x &= y | x = x & y
| ^= | x ^= y | x = x ^ y
| |= | x |= y | x = x | y

<section id="chapter12"></section>

> Logical Assigment Operators

| Operator | Example Usage | Meaning of
| -- | -- | --
| &&= | x &&= y | x = x && (x = y)
| ||= | x ||= y | x = x || (x = y)
| ??= | x ??= y | x = x ?? (x = y)

<section id="chapter13"></section>

> Escape Character

```js
var myString = "I am a "double quoted" string that inside " double quotes"";
```

As you can see in here, the __"__ double quote is a identifier where the string starts and ends. However, if you wish to use your double quote in string, you should use the escape character to prevent the string breakage.

```js
var myString = "I am a \" double quoted\" string that inside the \" double quotes\""
```

Escape character is __backslash \\__ . Here's the some example usage of escape character and using case.

|Code | View | Description
| -- | -- | --
| \\' | ' | Single Quote
| \\" | " | Double Quote
| \\\\ | \\ | Backslash
| \b | | Backspace
| \f | | Form Feed
| \n | | New Line
| \r | | Carriage Return
| \t | | Horizontal Tabulator
| \v | | Vertical Tabulator

<section id="chapter14"></section>

> String Identification

We already saw the string container for variable. Now we have variety way to contain string for variable. Here's the examples.

```js
var string_1 = "String with Double Quote";
var string_2 = 'String with Single Quote';
var string_3 = `String with Back Quote`;
```

That's just a way of preference. Of course there are certain advantages of each style since you can use less escape character for each. However, not that much of a difference.

<section id="chapter15"></section>

> String Operations

Finding the length of a string is one of the most used pre-function in programming. As we already learn by now is, string is a character array. And we may interested with how many character its contained in that string. In java script it is easy to find that via

```js
var myStr = "This is a testing script for length!";
console.log(myStr.length);
// 36
```

Apart from it, we can capture the character with given indexes like so

```js
var myStr = "This is a testing script for length!";

console.log(myStr[1]);
// h
console.log(myStr[myStr.length - 4]);
// g
```

From here we may confused like how the first character return __h__. Well this is because arrays start from 0 instead of 1. Which means when you type ```myStr[1]``` it's actually looking for the second letter/character in that string. There is no -1 index in array (for some reason. IDK), but we can access with length function and declaring from that.

Another unique future in JavaScript is individual characters are immutable in JavaScript. This is not the case in Python for example. I saw it first time in here. Here's an example of what I ment

```js
var myString = "Jello World";
myString[0] = "H";
console.log(myString);
// Jello World

myString = "Hello World";
console.log(myString);
// Hello World
```

<section id="chapter16"></section>

> Array Declaration

We already talk about array chars, _aka string_. But we didn't do any specific or complex array declaration for our data types. Arrays are ordered containers that can have one or more data type in it. You can store either singular or multiple data type in it.

```js
var myArray = ["John", "Doe", 25, "example@mail.com", True];
```

For this simple example, we can store any person firstname, lastname, age, mail and record(as boolean) at same array without any problem. But if doesn't required, we usually use same type data in one array for easier application like

```js
var strArray = ["Test", "Array", "Contains", "String"];
var intArray = [123, 234, 345, 456];
```

<section id="chapter17"></section>

> Nested Array Declaration

Nested arrays are simply array inside the arrays.

```js
var nestedArray = [[1,2,3], [4,5,6], [7,8,9], ['*', 0, '#']];
console.log(nestedArray[1][1]);
// 5
```

Also, we can consider the string arrays as nested arrays since the strings are already char arrays.

```js
var myArray = ["test", "array"];
console.log(myArray[1][3]);
// a
```

<section id="chapter18"></section>

> Accessing Array Element and Manipulating

Unlike strings, array elements can be changable with accessing individual characters.

```js
var testArray = [1, 3, 3, 4, 5];
testArray[1] = 2;

console.log(testArray);
// (5) [1, 2, 3, 4, 5]
```

That shown __(5)__ is length of array. This is related with the platfor you use for development. You may or may not see this future on your applied platform.

<section id="chapter19"></section>

> Manipulating Arrays with Push, Pop, Shift and Unshift Functions

There is usefull functions to add and remove manipulations to array.

```js
var myArray = ['Banana', 'Apple'];
var poppedData;
var shiftedData;
myArray.push('Pear');
console.log(myArray);
// ["Banana", "Apple", "Pear"]

removedData = myArray.pop();
console.log(removedData);
// Pear

shiftedData = myArray.shift();
console.log(shiftedData);
// Banana

myArray.unshift("Pear");
console.log(myArray);
// ["Pear", "Apple"]
```

If push using for adding new element, it will add to right placed (to last), or using pop to remove element it will remove the last item. You can also capture the popped item like in example. Shift function is similar to pop function, but now it's removing left placed (the first) item and it's also capturable like in example. Adding item to first place is also applicable with the function of unshift. The naming is a bit strange, but basically you can add first item to you array with unshift function like in example.

<section id="chapter20"></section>

> Creating own functions

In programming, it's vary common to use your own custom functions. It's a best practice to make your code DRY - [Don't Repeat Yourself](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself).

```js
function sayHelloTo(name){
  console.log("Hello to you " + name);
}

sayHelloTo("Jack");
sayHelloTo("John");
sayHelloTo("Julia");
// Hello to you Jack
// Hello to you John
// Hello to you Julia
```

With short explanation, function keyword is using for definition of a function. Next we give our function a name, in this case __sayHelloTo__ is our function name. And we passed one parameter function use that parameter inside our function.

<section id="chapter21"></section>

> Local and Global scopes for variables.

There is a concept that global and local variables. With words, local variable is only accessible in scope/block that's been written. On the other hand, global can be accessable from everywhere.

```js
var globalName = "Test 3";

function isItGlobal(){
  let nameVar = "Test 1";
  console.log(nameVar);
  console.log(globalName);
}

function nonGlobalScope(){
  let localVar = "Test 4";
  console.log(nameVar);
}

let nameVar = "Test 2";
isItGlobal();
nonGlobalScope();
console.log(nameVar);
console.log(globalName);
console.log(isThisOneGlobal);
console.log(localVar);

/* Output in Order
Test 1
Test 3
Test 2
Test 2
Test 3
Test 5
ReferenceError: localVar is not defined
*/
```

We already mention about difference [between let and var](https://sentry.io/answers/difference-between-let-and-var-in-javascript/#:~:text=The%20difference%20between%20let%20and,in%20which%20they're%20declared.) in previous [section](#chapter3). Example may conusing but I would like to address it in order

1. Test 1 -> This output come from local variable inside the __isItGlobal__ function.
1. Test 3 -> This output come from global variable inside the __isItGlobal__ function.
1. Test 2 -> This output comes from global declared variable inside the main javascript file. But called inside the __nonGlobalScope__ function.
1. Test 2 -> This one is captured from main javascript file. As you can see here, global variable nameVar doesn't manipulated from __isItGlobal__ function.
1. Test 3 -> This output captured from main javascript file with declaration in global scope.
1. Test 5 -> We declare this one without keyword of var/let which makes this variable global accessable for every functions.
1. Reference Error -> This one gives error since there is no __localVar__ definition in main javascript. Which mean local variable is out of scope.

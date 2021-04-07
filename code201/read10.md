## JavaScript book, Ch. 10, “Error Handling & Debugging”


JavaScript can be hard to learn and everyone makes
mistakes when writing it. This chapter will help you learn
how to find the errors in your code. It will also teach you how
to write scripts that deal with potential errors gracefully.
When you are writing JavaScript, do not expect to write it perfectly the first time.
Programming is like problem solving: you are given a puzzle and not only do you have to solve
it, but you also need to create the instructions that allow the computer to solve it. too.
When writing a long script, nobody gets everything right in their first attempt. The error
messages that a browser gives look cryptic at first, but they can help you determine what
went wrong in your JavaScript and how to fix it. In this chapter you will learn about:
THE CONSOLE &
DEV TOOLS
Tools built into the browser
that help you hunt for errors.
9 ERROR HANDLING & DEBUGGING
COMMON
PROBLEMS
Common sources of errors,
and how to solve them.
HANDLING
ERRORS
How code can deal with
potential errors gra cefully.




The JavaScript interpreter uses the concept of execution contexts.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope.


In the interpreter, each execution context has its own va ri ables object.
It holds the variables, functions, and parameters available within it.
Each execution context can also access its parent's v a ri ables object.
Functions in JavaScript are said to have lexical scope.
They are linked to the object they were defined within.
So, for each execution context, the scope is the
current execution context's variables object, plus the
variables object for each parent execution context.
var greeting = (function()
var d =new Date();
var time= d.getHours();
var greeting= greetUser{);
function greetUser() {
if (time < 12) {
var msg
else {
var msg
'Good morning ';
'Welcome ' ;
return= msg + getName();
funct i on getName() {
var name = 'Molly';
return name;
} ) ;
alert(greeting);
Imagine that each function is a nesting doll.
The children can ask the parents for information in
their variables. But the parents cannot get variables
from their children. Each child will get the same
answer from the same parent.



If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handling code.



Error objects can help you find where your mistakes are
and browsers have tools to help you read them.



If you understand execution contexts (which have two
stages) and stacks, you are more likely to find the error
in your code.
Debugging is the process of finding errors. It involves a
process of deduction.
The console helps narrow down the area in which the
error is located, so you can try to find the exact error.
JavaScript has 7 different types of errors. Each creates
its own error object, which can tell you its line number
and gives a description of the error.
If you know that you may get an error, you can handle
it gracefully using the try, catch, finally statements.
Use them to give your users helpful feedback.
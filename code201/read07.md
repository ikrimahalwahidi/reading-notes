# Chapter 6: “Tables” (pp.126-145)

There are several types of information
that need to be displayed in a grid or
table. For example: sports results, stock
reports, train timetables.
When representing information in a table, you need to think
in terms of a grid made up of rows and columns (a bit like a
spreadsheet). In this chapter you will learn how to:
Use the four key elements for creating tables
●● Represent complex data using tables
●● Add captions to tables.

A table represents information in a grid format.
Examples of tables include financial reports, TV
schedules, and sports results.

The <table> element is used to add tables to a web
page.
A table is drawn out row by row. Each row is created
with the <tr> element.
XX Inside each row there are a number of cells
represented by the <td> element (or <th> if it is a
header).
You can make cells of a table span more than one row
or column using the rowspan and colspan attributes.
For long tables you can split the table into a <thead>,
<tbody>, and <tfoot>.







# Chapter 3: “Functions, Methods, and Objects” (pp.106-144)

Browsers require very detailed instructions about what
we want them to do. Therefore, complex scripts can run
to hundreds (even thousands) of lines. Programmers use
functions, methods, and objects to organize their code.
This chapter is divided into three sections that introduce:
FUNCTIONS & OBJECTS BUILT-IN
METHODS OBJECTS
Functions consist of a In Chapter 1 you saw that The browser comes with
series of statements programmers use objects a set of objects that act
that have been grouped to create models of the like a toolkit for creating
together because they world using data, and that interactive web pages.
perform a specific task. objects are made up of This section introduces
A method is the same as a properties and methods. you to a number of built-in
function, except methods In this section, you learn objects, which you will
are created inside (and are how to create your own then see used throughout
part of) an object. objects using JavaScript. the rest of the book.


#### WHAT IS A FUNCTION?
Functions let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of st atements).
Grouping together the The steps that the function On the right, there is an example
statements that are required to needs to perform in order to of a function in the JavaScript
answer a question or perform a perform its task are packaged file. It is called updateMessage () .
task helps organize your code. up in a code block. You may
remember from the last chapter Don't worry if you do not
Furthermore, the statements in a that a code block consists of one understand the syntax of the
function are not always executed or more statements contained example on the right; you will
when a page loads, so functions within curly braces. (And you do take a closer look at how to wri te
also offer a way to store the steps not write a semicolon after the and use functions in the pages
needed to achieve a task. The closing curly brace - like you do that follow.
script can then ask the function after a statement.)
to perform all of those steps as Remember that programming
and when they are required. Some functions need to be languages often rely upon on
For example, you might have provided with information in name/value pairs. The function
a task that you only want to order to achieve a given task. For has a name, updateMessage,
perform if the user clicks on a example, a function to ca lculate and the value is the code block
specific element in the page. the area of a box would need (which consists of statements).
to know its width and height. When you call the function by its
If you are going to ask the Pieces of information passed name, those statements will run.
function to perform its task to a function are known as
later, you need to give your parameters. You can also have anonymous
function a name. That name functions. They do not have a
should describe the task it is When you write a function and name, so they cannot be called.
performing. When you ask it to you expect it to provide you Instead, they are executed as
perform its task, it is known as with an answer, the response is soon as the interpreter comes
ca lling the function. known as a return value. across them.


Functions allow you to group a set of related
statements together that represent a single task.

Functions can take parameters (informatiorJ required
to do their job) and may return a value.

An object is a series of variables and functions that
represent something from the world around you.

In an object, variables are known as properties of the
object; functions are known as methods of the object.

Web browsers implement objects that represent both
the browser window and the document loaded into the
browser window.

JavaScript also has several built-in objects such as
String, Number, Math, and Date.

Their properties and
methods offer functionality that help you write scripts.

Arrays and objects can be used to create complex data
sets (and both can contain the other).
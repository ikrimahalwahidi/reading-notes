
# Chapter 3: “Object Literals” (pp.100-105)

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
calling the function. known as a return value. across them.







Expressions produce a value. They can be used where values are expected.
If a function is placed where a browser expects to see an expression,
(e.g., as an argument to a function), then it gets treated as an expression.
FUNCTION DECLARATION
A function declaration creates a function that you
can ca ll later in your code. It is the type of function
you have seen so far in this book.
In order to call the function later in your code, you
must give it a name, so these are known as named
functions. Below, a function called area() is
declared, which can then be called using its name.
function area (width, height)
return width * height;
};
var size= area(3, 4) ;
As you will see on p456, the interpreter always
looks for variables and function declarations before
going through each section of a script, line-by -line.
This means that a function created with a function
declaration can be ca lled before it has even been
declared.
For more information about how variables and
functions are processed first, see the discussion
about execution context and hoisting on
p452 - p457.
§ FUNCTIONS, METHODS & OBJECTS
FUNCTION EXPRESSION
If you put a function where the interpreter would
expect to see an expression, then it is treated as an
expression, and it is known as a function expression.
In function expressions, the name is usually omitted.
A function with no name is called an anonymous
function. Below, the function is stored in a variable
called area. It can be called like any function created
with a function declaration.
var ar ea = f unction(width, height) {
r eturn width * height;
} ;
var size = area(3, 4) ;
In a function expression, the function is not
processed until the interpreter gets to that
statement. This means you cannot call this function
before the interpreter has discovered it. It also means
that any code that appears up to that point could
potentially alter what goes on inside this function.







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
String, Number, Math, and Date. Their properties and
methods offer functionality that help you write scripts.
Arrays and objects can be used to create complex data
sets (and both can contain the other).










# Chapter 5: “Document Object Model” (pp.183-242)




The Document Object Model (DOM) specifies
how browsers should create a model of an HTML
page and how JavaScript can access and update the
contents of a web page while it is in the browser window.
The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules.
It is implemented by all major browser makers, and covers two primary areas:
MAKING A MODEL OF THE
HTML PAGE
When the browser loads a web page, it
creates a model of the page in memory.
The DOM specifies the way in which the
browser should structure this model using
a DOM tree.
The DOM is called an object model
because the model (the DOM tree) is
made of objects.
Each object represents a different part of
the page loaded in the browser window.
s DOCUMENT OBJECT MODEL
ACCESSING AND CHANGING
THE HTML PAGE
The DOM also defines methods and
properties to access and update each
object in this model, which in turn updates
what the user sees in the browser.
You will hear people call the DOM an
Application Programming Interface (API).
User interfaces let humans interact with
programs; APls let programs (and scripts)
talk to each other. The DOM states what
your script can "ask the browser about the
current page, and how to tell the browser
to update what is being shown to the user.
As a browser loads a web page, it creates a model of that page.
The model is called a DOM tree, and it is stored in the browsers' memory.
It consists of four main types of nodes.
BODY OF HTML PAGE
<html>
<body>
<di v id="page">
<hl id="header">List</hl>
<h2>Buy groceries</h2>
<ul>
<li id="one" class="hot"><em>fresh</em> figs</li>
<li id="two" class="hot">pine nuts</l i>
<l i id="three" class="hot">honey</l i>
<l i id="four">balsamic vinegar</l i>
</ ul>
<script src="js/list. js "></scri pt>
</ div>
</ body>
</ html>





The browser represents the page using a DOM tree.
DOM trees have four types of nodes: document nodes,
element nodes, attribute nodes, and text nodes.
You can select element nodes by their id or cl ass
attributes, by tag name, or using CSS selector syntax.
Whenever a DOM query can return more than one
node, it will always return a Nadel ist.
From an element node, you can access and update its
content using properties such as text Content and
inner.HTML or using DOM manipulation techniques.
An element node can contain multiple text nodes and
child elements that are siblings of each other.
In older browsers, implementation of the DOM is
inconsistent (and is a popular reason for using jQuery).
Browsers offer tools for viewing the DOM tree .





## Chapter 7: “Forms” (p.144-175)


Traditionally, the term 'form' has referred
to a printed document that contains
spaces for you to fill in information.
HTML borrows the concept of a form to refer to different
elements that allow you to collect information from visitors to
your site.
Whether you are adding a simple search box to your website or
you need to create more complicated insurance applications,
HTML forms give you a set of elements to collect data from
your users. In this chapter you will learn:
How to create a form on your website
The different tools for collecting data
New HTML5 form controls.


A form may have several form controls, each
gathering different information. The server
needs to know which piece of inputted data
corresponds with which form element.
To differentiate between various pieces of inputted data, information
is sent from the browser to the server using name/value pairs. In this
example, the form asks for the visitor's username and also for their
favorite jazz musician. The name/value pairs sent to the server are:
You should never change the name of a form control in a page unless
you know that the code on the server will understand this new value.
username=Ivy
If the form control allows the
user to enter text, then the value
of the form control is whatever
the user has typed in.
vote=Herbie
If the form control allows you
to choose from a fixed set of
answers (e.g. radio buttons,
checkboxes or a drop down list),
the web page author will add
code that gives each option an
automatic value.
username=Ivy
Name
Value


Whenever you want to collect information from
visitors you will need a form, which lives inside a
<form> element.
Information from a form is sent in name/value pairs.
Each form control is given a name, and the text the
user types in or the values of the options they select
are sent to the server.
HTML5 introduces new form elements which make it
easier for visitors to fill in forms.





## Chapter 6: “Events” (pp.243-292)


When you browse the web, your browser registers different
types of events. It's the browser's way of saying, "Hey, this
just happened." Your script can then respond to these events.
Scripts often respond to these events by updating the content of the web page (via the
Document Object Model) which makes the page feel more interactive. In this chapter, you
will learn how:
INTERACTIONS EVENTS TRIGGER CODE RESPONDS
CREATE EVENTS CODE TO USERS
Events occur when users When an event occurs, In the last chapter, you
click or tap on a link, hover or fires, it can be used saw how the DOM can
or swipe over an element, to trigger a particular be used to update a page.
type on the keyboard, function. Different code The events can trigger the
resize the window, or can be triggered when -kinds of changes the DOM
when the page they users interact with is capable of. This is how a
requested has loaded. different parts of the page. web page reacts to users.
l ~ I .


DIFFERENT EVENT TYPES
Here is a selection of the events that occur in the browser while you are
browsing the web. Any of these events can be used to trigger a function
in your JavaScript code.
UIEVENTS Occur when a user interacts with the browser's user interface (UI) rather than the web page
EVENT DESCRIPTION
load Web page has finished loading
unload Web page is unloading (usually because a new page was requested)
error Browser encounters a JavaScript error or an asset doesn't exist
resize Browser window has been resized
scroll User has scrolled up or down the page
KEYBOARD EVENTS Occur when a user interacts with the keyboard (see also input event)
EVENT DESCRIPTION
keydown User first presses a key (repeats while key is depressed)
keyup User releases a key
keypress Character is being inserted (repeats while key is depressed)
MOUSE EVENTS Occur when a user interacts with a mouse. trackpad, or touchscreen
EVENT DESCRIPTION
click User presses and releases a button over the same element
dbl click User presses and releases a button twice over the same element
moused own User presses a mouse button while over an element
mouseup User releases a mouse button while over an element
mousemove User moves the mouse (not on a touchscreen)
mouseover User moves the mouse over an element (not on a touchscreen)
mouseout User moves the mouse off an element (not on a touchscreen)



HOW EVENTS TRIGGER
JAVASCRIPT CODE
When the user interacts with the HTML on a web page, there are three
steps involved in getting it to trigger some JavaScript code.
Together these steps are known as event handling.
1
Select t he element
node(s) you want the
script to respond to.
For example, if you want to
trigger a function when a user
clicks on a specific link, you need
to get the DOM node for that
link element. You do this using a
DOM query (see Chapter 5).
The UI events that relate to the
browser window (rather than the
HTML page loaded in it) work
with the window object rather
than an element node. Examples
include the events that occur
when a requested page has
f inished loading, or when the
user scrolls. You will learn about
using these on p272.
8 EVENTS
2
Indicate which event on
the selected node(s) will
trigger the response.
Programmers call this binding an
event to a DOM node.
The previous two pages showed
a selection of the popular events
that you can monitor for.
Some events work with most
element nodes, such as the
mouseover event, which is
triggered when the user rolls
over any element. Other events
only work with specific element
nodes, such as the submit event,
which only works with a form.
3
State the code you want
to run when the event
occurs.
When the event occurs, on a
specified element, it will trigger
a function. This may be a named
or an anonymous function.





Events are the browser's way of indicating when
something has happened (such as when a page has
finished loading or a button has been clicked).
Binding is the process of stating which event you are
waiting to happen, and which element you are waiting
for that event to happen upon.
When an event occurs on an element, it can trigger a
JavaScript function. When this function then changes
the web page in some way, it feels interactive because
it has responded to the user.
You can use event delegation to monitor for events
that happen on all of the children of an element.
The most commonly used events are W3C DOM
events, although there are others in the HTMLS
specification as well as browser-specific events.





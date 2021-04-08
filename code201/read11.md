
### Chapter 16: “Images” (pp.406-427)

Controlling the size and alignment of
your images using CSS keeps rules that
affect the presentation of your page in
the CSS and out of the HTML markup.
You can also achieve several interesting effects using
background images. In this chapter you will learn how to:
Specify the size and a ●● lignment of an image using
Add background images to boxes
Create image rollovers in CSS.



Article
img.large {
width: 500px;
height: 500px;}
img.medium {
width: 250px;
height: 250px;}
img.small {
width: 100px;
height: 100px;}
CSS
<img src="images/magnolia-large.jpg"
class="large" alt="Magnolia" />
<img src="images/magnolia-medium.jpg"
class="medium" alt="Magnolia" />
<img src="images/magnolia-small.jpg"
class="small" alt="Magnolia" />
chapter-16/image-sizes.html HTML
You can control the size of an
image using the width and
height properties in CSS, just
like you can for any other box.
Specifying image sizes helps
pages to load more smoothly
because the HTML and CSS
code will often load before the
images, and telling the browser
how much space to leave for an
image allows it to render the rest
of the page without waiting for
the image to download.
You might think that your site
is likely to have images of all
different sizes, but a lot of sites
use the same sized image across
many of their pages.
For example, an e-commerce site
tends to show product photos
at the same size. Or, if your site
is designed on a grid, then you
might have a selection of image
sizes that are commonly used on
all pages, such as:
Small portrait: 220 x 360
Small landscape: 330 x 210
Feature photo: 620 x 400
Whenever you use consistently
sized images across a site,
you can use CSS to control
the dimensions of the
images, instead of putting the
dimensions in the HTML.

You can specify the dimensions of images using CSS.
This is very helpful when you use the same sized
images on several pages of your site.
Images can be aligned both horizontally and vertically
using CSS.
You can use a background image behind the box
created by any element on a page.
 Background images can appear just once or be
repeated across the background of the box.
 You can create image rollover effects by moving the
background position of an image.
 To reduce the number of images your browser has to
load, you can create image sprites.




### Chapter 19: “Practical Information” (476-492)


To wrap up the book we are going to look
at some practical information that will
help you launch a successful site.
There are entire books written about each of the topics
covered in this chapter but I will introduce you to the key
themes that each subject deals with and give you pointers for
what you need to be considering. You will see:
The basics of search e ●● ngine optimization
Using analytics to understand how people are using your
site after it has launched
Putting your site on the web.

SEO is a huge topic and several books have been written on the subject.
The following pages will help you understand the key concepts so you can
improve your website's visibility on search engines.

The Basics
Search engine optimization (or
SEO) is the practice of trying
to help your site appear nearer
the top of search engine results
when people look for the topics
that your website covers.
At the heart of SEO is the idea of
working out which terms people
are likely to enter into a search
engine to find your site and then
using these terms in the right
places on your site to increase
the chances that search engines
will show a link to your site in
their results.
In order to determine who comes
first in the search results, search
engines do not only look at what
appears on your site. They also
consider how many sites link
to you (and how relevant those
links are). For this reason, SEO
is often split into two areas:
on-page techniques and off-page
techniques.
On-Page Techniques
On-page techniques are the
methods you can use on your
web pages to improve their
rating in search engines.
The main component of this is
looking at keywords that people
are likely to enter into a search
engine if they wanted to find
your site, and then including
these in the text and HTML code
for your site in order to help the
search engines know that your
site covers these topics.
Search engines rely very heavily
on the text that is in your pages
so it is important that the terms
people are going to search for
are in text. There are seven
essential places where you want
your keywords to appear.
Ensuring that any images have
appropriate text in the value of
their alt attribute also helps
search engines understand the
content of images.
Off-Page Techniques
Getting other sites to link to you
is just as important as on-page
techniques. Search engines help
determine how to rank your
site by looking at the number of
other sites that link to yours.
They are particularly interested
in sites whose content is related
to yours. For example, if you
were running a website that
sold fish bait, then a link from
a hairdresser is not likely to be
considered as relevant as one
from an angling community.
Search engines also look at the
words between the opening
<a> tag and closing </a> tag
in the link. If the text in the link
contains keywords (rather than
just click here or your website
address) it may be considered
more relevant.
The words that appear in links to
your site should also appear in
the text of the page that the site
links to.

Search engine optimization helps visitors find your
sites when using search engines.
Analytics tools such as Google Analytics allow you to
see how many people visit your site, how they find it,
and what they do when they get there.
XX To put your site on the web, you will need to obtain a
domain name and web hosting.
FTP programs allow you to transfer files from your
local computer to your web server.
Many companies provide platforms for blogging, email
newsletters, e-commerce and other popular website
tools (to save you writing them from scratch).
# Chapter 4: Ch.4 “Links” (pp.74-93)

Links are created using the <a> element.
The <a> element uses the href attribute to indicate
the page you are linking to.
If you are linking to a page within your own site, it is
best to use relative links rather than qualified URLs.
You can create links to open email programs with an
email address in the "to" field.
You can use the id attribute to target elements within
a page that can be linked to.
  
  Writing Links
<a href="http://www.imdb.com">IMDB</a>
This is the page the
link takes you to
Opening link tag
This is the text the
user clicks on
Closing
link tag
LINKS 78
The text between the opening
<a> tag and closing </a> tag
is known as link text. Where
possible, your link text should
explain where visitors will be
taken if they click on it (rather
than just saying "click here").
Below you can see the link to
IMDB that was created on the
previous page.
Many people navigate websites
by scanning the text for links.
Clear link text can help visitors
find what they want. This
will give them a more positive
impression of your site and may
encourage them to visit it for
longer. (It also helps people
using screen reader software.)
To write good link text, you can
think of words people might
use when searching for the
page that you are linking to.
(For example, rather than write
"places to stay" you could use
something more specific such as
"hotels in New York.")
79 LINKS
Result
<p>Movie Reviews:
<ul>
<li><a href="http://www.empireonline.com">
Empire</a></li>
<li><a href="http://www.metacritic.com">
Metacritic</a></li>
<li><a href="http://www.rottentomatoes.com">
Rotten Tomatoes</a></li>
<li><a href="http://www.variety.com">
Variety</a></li>
</ul>
</p>
chapter-04/linking-to-<a> other-sites.html HTML
Links are created using the <a>
element which has an attribute
called href. The value of the
href attribute is the page that
you want people to go to when
they click on the link.
Users can click on anything that
appears between the opening
<a> tag and the closing </a>
tag and will be taken to the page
specified in the href attribute.
When you link to a different
website, the value of the href
attribute will be the full web
address for the site, which is
known as an absolute URL.
Browsers show links in blue with
an underline by default.
Linking to Other Sites
URL stands for Uniform
Resource Locator. Every web
page has its own URL. This is the
web address that you would type
into a browser if you wanted to
visit that specific page.
An absolute URL starts with
the domain name for that site,
and can be followed by the path
to a specific page. If no page is
specified, the site will display the
homepage.
Absolute UR Ls
Article
LINKS 80
Result
<a>
When you are linking to other
pages within the same site,
you do not need to specify the
domain name in the URL. You
can use a shorthand known as a
relative URL.
If all the pages of the site are in
the same folder, then the value
of the href attribute is just the
name of the file.
If you have different pages of a
site in different folders, then you
can use a slightly more complex
syntax to indicate where the
page is in relation to the current
page. You will learn more about
these on the pages 81-84.
If you look at the download
code for each chapter, you will
see that the index.html file
contains links that use relative
URLs.
Relative URLs help when building
a site on your computer because
you can create links between
pages without having to set up
your domain name or hosting.
<p>
<ul>
<li><a href="index.html">Home</a></li>
<li><a href="about-us.html">About</a></li>
<li><a href="movies.html">Movies</a></li>
<li><a href="contact.html">Contact</a></li>
</ul>
</p>
HTML chapter-04/linking-to-other-pages.html
Linking to Other Pages
on the Sa me Site
When linking to other pages
within the same site, you can
use relative URLs. These are like
a shorthand version of absolute
URLs because you do not need
to specify the domain name.
We will take a closer look at
relative URLs on pages 83-84
as there are several helpful
shortcuts you can use to write
links to other pages on your own
website.
  
 # Chapter 15: “Layout” (pp.358-404)
  
 <div> elements are often used as containing elements
to group together sections of a page.
 Browsers display pages in normal flow unless you
specify relative, absolute, or fixed positioning.
The float property moves content to the left or right
of the page and can be used to create multi-column
layouts. (Floated items require a defined width.)
Pages can be fixed width or liquid (stretchy) layouts.
Designers keep pages within 960-1000 pixels wide,
and indicate what the site is about within the top 600
pixels (to demonstrate its relevance without scrolling).
Grids help create professional and flexible designs.
CSS Frameworks provide rules for common tasks.
You can include multiple CSS files in one page.
  Possible Layouts:
960 Pixel wide
12 Column Grid
940 px
460 px
300 px
220 px
140 px
460 px
300 px 300 px
220 px 220 px 220 px
140 px 140 px 140 px 140 px 140 px

  

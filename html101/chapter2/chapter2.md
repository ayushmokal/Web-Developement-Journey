08. Blueprint

# HTML Structure
Now that we know how to spin up a web page, let's get back to the basics and explore how to structure our HTML files better. 📄

Here are some must-haves in a .html file!

The <!DOCTYPE html> is the document type declaration that appears at the top of a .html file and tells the browser that our file is written in HTML5. This is used with a <html> element containing all the code processed on the page.

Notice how the <!DOCTYPE html> doesn’t have a closing tag, while <html> does.

<!DOCTYPE html>
<html>
  Code goes here
</html>

Note: All HTML files must start with a <!DOCTYPE html> declaration and the <html> element.

We skipped them in the first chapter, but they are essential parts of every HTML file.

<!DOCTYPE html>
<html>
  <head>
    Some code goes here
  </head>
  <body>
    A lot more goes here
  </body>
</html>

Inside <html>, there should be two elements:

<head>: This contains all the info for your browser that's not visible on the page.
<body>: This contains all of the content that you will end up seeing on the page.
The <title> element goes in the <head> and assigns text to the tab in our browser.

This is what the browser tab looks like when you visit codedex.io:


The code for this would be:

<!DOCTYPE html>
<html>
  <head>
    <title>Codédex | Start your coding adventure ⋆˙⟡</title>
  </head>
  <body>
    Code goes here
  </body>
</html>


09. Family Tree
# Parents & Children
The elements in our HTML file are arranged much like a family tree. Most individual elements can be parents with one or more child elements.

For example:

<!DOCTYPE html>
<html>
  <head>
    <title>My Web Page</title>
  </head>
  <body>
    <p>Well, <i>howdy</i> there!</p>
  </body>
</html>

Here are some relationships:

<head> and <body> are children of <html>.
<title> is the child of <head>.
<i> is child of <p> and grandkid of <body>.
Now, what’s the relationship between <i> and <title>? Haha kidding.

# Siblings
Elements can also be siblings if they share a direct parent element. Take this unordered list, for instance:

<body>
  <ul>
    <li>🍄 Mario</li>
    <li>🐢 Luigi</li>
  </ul>
</body>

The two <li> elements are siblings because both are children of the same parent, the <ul> element.

10. Craigslist Ad
# Comments
Comments are useful for taking notes about the logic and intentions behind different parts of our web page. They help us understand what our code is doing, especially if it was written a while ago.

Not only should comments benefit whoever wrote the code, but they should also be helpful to anyone reviewing it later.

How do we comment in HTML? It’s simple:

<!-- I am a comment. -->
<p>And I'm not a comment!</p>

Everything surrounded by the <!-- and --> comment markers is ignored and not rendered on the browser:

<!-- Let’s make you a comment, too. -->
<!-- <p>Nooo!</p> -->

# Inline vs. Multi-line
Comments are super flexible because they can span multiple lines:

<!--
  This is also a comment.
-->

They can also be used within an element:

<p>This text is visible. <!-- But this is not. --></p>

Note: It isn't recommended that you be excessive with comments. They should be used sparingly and removed when no longer needed.

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


15. Google

# What are Forms?

What do sign up, login, and checkout pages have in common? They all collect user input data! 📋

In this chapter, we're going to learn how to take input from the user with forms!

Forms come in every shape and form (pun intended). From buying something online to using a search engine, forms are a part of everyday digital life.

They're pretty straight-forward:

The user enters some information.
The user presses a “Submit” button.
And something happens!
For example, searching on Wikipedia is just filling out and submitting a form:


To create a form in HTML, we can use the <form> element:

<form action="" method="">
  <!-- More code will go here -->
</form>

Two attributes are commonly used with the <form> element:

The action attribute that says where the form data should go after it is submitted.
The method attribute for how the form data is processed.
It is usually either sent somewhere else via "post" or used with something else via "get".

Note: For the rest of this chapter, the action and method attributes will not be featured in the examples. Not to worry, though! The forms will still render just fine. 😀

# Inputs

But wait… how do we even enter the form data? How do we submit it?

In HTML forms, we use the <input> element as an interactive control for entering data. A type attribute is used to determine the kind of input to use. While there are many types of inputs, the two we'll use most often are:

A text value that renders a plain textbox on the form.
<form>
  <input type="text">
</form>

A submit value that turns the <input> element into a button for submitting the form data.
<form>
  <input type="submit">
</form>

Note: The <input> element uses a self-closing tag.

This is what both look like in a <form> element:

Submit Input

By default, the text of the "submit" input type will say "Submit", but this can be changed by setting a value attribute for the <input> element:

<input type="submit" value="Submit Form!">

This is what the altered "submit" input now looks like:

refer google.html ( where we implemented the google search form )


16. Sign Up v1
# Input Type: Emails
There are many other <input> types in forms.

Besides plain text, we can set an input type for email:

<input type="email">

This tells the form to expect a text input with the typical email syntax (including the @ symbol).

# Input Type: Passwords
There is also an <input> element type for passwords:

<input type="password">

Dots will replace the text that would otherwise appear in the text box:

Password Input


17. Sign Up v2
# Input Validation
By now, we've explored different types of inputs for HTML forms.

But how do we make sure that the right data is going into the form? For example, if a form asks for an email, how can it tell that the input is a valid email that includes the @ symbol?

HTML forms actually have a few tools for this!

For example, the "email" type checks if the submitted input is a valid email address:

Email Validation

Forms can also mask text input if the <input> element has a "password" type. We can even give it a minlength and maxlength attribute to further validate the input:

<input type="password" minlength="4" maxlength="10">

If we render this:

Password Validation

We also can't type past 10 characters (via maxlength) and a message appears if we submit less than 4 characters.

# Required Data
Oftentimes, forms need input in order to be submitted.

The required attribute can be applied to one or more form inputs to enforce this.

<form method="dialog">
  Name: <input type="text" required>
  <br><br>
  Favorite Color: <input type="text">
  <input type="submit">
</form>

The<input> element for a "Name" is marked with the required attribute.

Here is what happens when submitting without filling out this input:

18. RSVP
# Input Type: Number
There may be times when numbers may be involved in forms. This could be anything from a person's age to the number of items bought at a store.

To prompt the <input> element for numbers, we do the following:

<input type="number">

Try it out! Type a number in the bow below:

When the cursor hovers above this input, "up" and "down" arrow buttons appear on the right side.

By default, selecting these buttons moves the numeric value up or down by 1. However, a step attribute can be used to change this:

<input type="number" step="2">

This renders the following:

So instead of the input value going up or down by 1, it goes up or down by 2.

Additionally, a max and min attribute can be used to set how high or low this input can go:

<input type="number" min="1" max="42">

This is the rendered output:

# Input Type: Checkbox and Radio
There are also input types that allow us to make one or more choices from a list of options. Two of them are "checkbox" and "radio".

The "checkbox" type renders as a box that is ticked off to mark the input as "finished" or "complete."

<h3>Favorite Movie Genres</h3>
<input type="checkbox"> Action<br>
<input type="checkbox"> Sci-Fi<br>
<input type="checkbox"> Rom-Com<br>
<input type="checkbox"> K-Drama<br>
<input type="checkbox"> Documentary<br>

The code above renders this:

We can check off multiple items with this input type.

Next, there's the "radio" button type. Like with checkboxes, radio buttons are lists of options. However, only one option can be selected.

Here's an example that highlights a recent popular illusion:

<h3>Which do you think?</h3>
<input type="radio"> Yanny
<br>
<input type="radio"> Laurel

This is what the rendered inputs look like:

Wait a second... it can't be both "Yanny" and "Laurel", right? Shouldn't only one option be selected at a time?

The way to make this so is by assigning a matching name attribute to each "radio" input type. This puts them in the same group of options to choose from.

<h3>Which do you think?</h3>
<input type="radio" name="option"> Yanny
<br>
<input type="radio" name="option"> Laurel

The output should now work as expected:

19. Contact Us

# Textareas
Another popular kind of text input in forms are text areas.

The <textarea> element renders as a plain, mini-text editor on the web page.

<textarea id="data-entry" rows="7" cols="42"  placeholder="Enter some data here!"></textarea>

When rendered, it looks like this:

In addition to class and id, the <textarea> uses the following attributes:

rows: The amount of visible rows, or text lines (defaulting at 2).
cols: The number of visible columns in average character widths (defaulting at 20).
placeholder: Some default text meant to explain what kind of data should be entered.
The required attribute can be applied to the <textarea> element, too.

# Form Labels
In HTML, labels can be used in forms to associate pieces of text with form controls and inputs.

The <label> element is used for this:

<form>
 <label>Book Title: </label><input type="text">
 <br><br>
 <label>Author: </label><input type="text">
 <br><br>
 <input type="submit">
</form>

The rendered input looks like:

In order to associate <label> elements to form inputs, its for attribute must match the id of a given <input> element:

<form>
 <label for="title">Book Title: </label><input type="text" id="title">
 <br><br>
 <label for="author" >Author: </label><input type="text" id="author">
 <br><br>
 <input type="submit">
</form>

Alternatively, these associations can be implicitly defined:

<form>
  <label>Book Title: <input type="text"></label>
  <label>Author: <input type="text"></label>
</form>

This will render the exact same form.


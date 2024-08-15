1) # What is HTML?
Welcome to The Origins Trilogy! The beginning of your web development journey. 🌋

The language we are learning is HTML, or HyperText Markup Language. It was created by a developer named Tim Berners-Lee in 1991.

Today, every website in the world uses HTML!

However, HTML is just one piece that is used to build a web page. Most web pages use:

Html LogoHTML: Create the website skeleton.
JavaScript BadgeCSS: Modify the website presentation.
JavaScript BadgeJavaScript: Make it interactive.
This course will focus on HTML. We want to build a strong foundation before moving on.

As the name suggests, HTML is a markup language; it marks up every piece of content on a web page and defines its type. The language is simple and perfect for beginners!

All the programs we write will be HTML files with the file extension .html.


02. Elemental

To understand how HTML works, we need to start with elements – the smallest building blocks of the language.

An element usually consists of an opening tag, the content, and a closing tag. A tag is enclosed in angle brackets.

<p>Hello World!</p>

So this is one HTML element where:

<p> is the opening tag.
Hello World! is the content.
</p> is the closing tag.
The <p> paragraph element tells the browser that the content inside is "paragraph" text.

Let's take a look at a basic HTML program that displays a message in the browser:

<body><p>👋 I'm a new web developer!</p></body>

The <body> element defines an HTML document's "body" and it's where any content that we want to display to the user will be held:

<body> opening tag begins the "body".
<p>👋 I'm a new web developer!</p> is some text in a paragraph element.
</body> closing tag ends the "body".
Note: There can only be one <body> element in an HTML file.


# Indentation
While indenting HTML code isn't required, doing so is good practice because it makes your code easier to read and visualize the nesting levels.

Here's how to indent the previous code block:

<body>
  <p>👋 I'm a new web developer!</p>
</body>

Notice how it's a lot easier to read this way!

We recommend two spaces for indentations.

03. Newspaper

# Headings
Let's look at some more elements.

Suppose we want to add a headline to our website that displays a news article. Here's how we would do it using a <h1> heading element and a <p> paragraph element:

<body>
  <h1>Breaking News</h1>
  <p>Florida man robs convenience store with an alligator. Leaves a baby Crocs behind.</p>
</body>

There are six levels of section headings, from <h1> to <h6>:

<h1>Heading level 1</h1>
<h2>Heading level 2</h2>
<h3>Heading level 3</h3>
<h4>Heading level 4</h4>
<h5>Heading level 5</h5>
<h6>Heading level 6</h6>

# Line Break
Suppose we also want to add a new line within a paragraph element. Pressing enter won't do us any good because HTML ignores multiple spaces and line breaks within elements.

So we must use the <br> break tag here!

The <br> break tag adds a line break:
<body>
  <h1>Breaking News</h1>
  <p>Florida man robs convenience store with an alligator.<br>Leaves a baby Crocs behind.</p>
</body>
A self-closing tag doesn't need to be closed manually by a closing tag (i.e., it does not have a separate closing </tag>). The break tag is the first one we have encountered.

The final code will become:


04. Corporate Talk

# Text Formatting
Now that we know how to display basic text, how do we bold sentences, italicize new words, underline important phrases, and more?

To do that, we need text formatting elements! They make default texts look fancier.

Here are some common ones:

<b> element to bold text.
<i> element to italicize text.
<u> element to underline text.
<s> element to strikethrough text.</s>
This is how they are used:

<b>This text is using bold formatting.</b><br>
<i>This text is using italics formatting.</i><br>
<u>This text is using underline formatting.</u><br>
<s>This text is using strikethrough formatting.</s><br>

Note: The <b> element is just for bolding text stylistically; HTML also has a <strong> element used to convey that the content inside is important, as well as styling it to be bold.

Here are all four tags in action in a classroom announcement:

05. Sous-Chef
# Lists
Lists are a great way to manage time, figure out what needs to be done, and remember things. And it feels good when we check items off!

We will learn about two types of HTML lists:

<ul> Unordered lists
<ol> Ordered lists
For unordered lists, also known as bullet points, start with the <ul> tag and wrap each item in a <li> list item element. Like so:

<ul>
  <li>🧺 Go to laundromat.</li>
  <li>🖥 Code for 45 min.</li>
  <li>💅 Take a bubble bath.</li>
</ul>


The <ul> is great for listing things in any order. But what if we wanted to number the list?

For ordered lists, also known as numbered lists, we use the <ol> element:


<ol>
  <li>🧺 Go to laundromat.</li>
  <li>🖥 Code for 45 min.</li>
  <li>💅 Take a bubble bath.</li>
</ol>


06. Lost Pet

# Links

The first website ever created in 1991 is still live today: TheProject.html.

What do you notice? Besides the fact that it is bare-boned, there are a bunch of links!

Links are integral to the idea of the internet. They are the primary way users connect to other sites and navigate the web.

So how do we add a link to our web page?

We can use the <a> anchor element! This link tag allows us to add a hyperlink to a piece of text. Let's see how we can do this:

<a href="https://archive.org/web">Internet Archive</a>

Here, the <a> anchor element is similar to other tags, where the text inside is what is displayed. But what about the href inside the opening tag?

An href, or hyperlink reference, is a reference or pointer to another website that is linked in our HTML. When the text “Internet Archive” is clicked, the HTML will redirect to that site, which in our case, is https://archive.org/web!

Note: This can also be used to point to an email or phone number using a mailto:, tel:, or sms: parameter, respectively.

<a href="mailto:frankie@gmail.com">📧</a>
<a href="tel:640-500-CODE">☎️</a>
<a href="sms:320-250-HTML">💬</a>

<a herf="mailto:ayushmokal13@gmail.com">📧</a>


# Images

What if we want to add images? We can use a similar format, but with the <img> image element.

<p>Here's a cute pic:</p>
<img src="https://i.redd.it/5unn16axx1v81.jpg">


The <img> image element is another self-closing tag, so it doesn't have a closing tag.

src attribute, which stands for “source”, specifies the file path of the image.
"https://i.redd.it/5unn16axx1v81.jpg" is the image path.
For most images, the file path can be found by right-clicking on the image and selecting "Copy Image Address".


<h2>Woohoo! (╥﹏╥)</h2>
<p>You've reached the end of chapter 1 🫶</p>

Here's a refresher on what we went over:

HTML elements, tags, and indentation.
Headings, paragraphs, and break tags: <h1>-<h6>, <p>, <br>.
Text formatting: <b>, <i>, <u>, <s>.
Unordered and ordered lists: <ul>, <ol>.
Links and images: <a>, <img>.

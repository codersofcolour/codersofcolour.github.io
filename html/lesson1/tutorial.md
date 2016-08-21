---
layout: page
title: HTML & CSS Lesson 1
---

## Introduction to HTML

### Objectives 

In this tutorial we are going to look at:

* What is HTML?
* What is an element?
* Webpage structure
* Fundamental HTML elements
* Special HTML characters
* HTML commenting

### Goal

By the end of this tutorial you will have built [a webpage about someone who inspires you.](http://codebar.github.io/tutorials/html/lesson1/example.html "All About Beyonce"). We will use Beyonce in this tutorial, but you are encouraged to create a webpage about any person who inspires you.

#### What is HTML?

**HTML** is the language used to build websites. All text and content that you see on the internet is built using HTML. 

**CSS** is used with HTML to style the page. However we will not be learning any of this today as this is covered in the next tutorial.


#### What does HTML stand for?

**H**yper **T**ext **M**arkup **L**anguage


## HTML elements

An **element** is an HTML building block. There are paragraphs, headings, links, lists, and [many more.](https://developer.mozilla.org/en/docs/Web/HTML/Element)

HTML elements are made up of an opening tag, followed by content then the closing tag.

`<tagname>some content</tagname>`

Some HTML elements do not need a closing tag as they are used to place standalone elements on the webpage. For example:

```html
<hr>
<img>
```

## Webpage structure

The doctype is the first thing that must be defined in an HTML page.
It tells the browser which version of HTML the page is using.

```html
<!DOCTYPE html>
```

We will only be using html for now, but you can find more about doctypes [here](http://www.w3.org/wiki/Doctypes_and_markup_styles).

The doctype is always followed by the `<html>` tag, which contains the contents of your page.

```html
<!DOCTYPE html>
<html>
</html>
```

### HEAD and BODY tags

A HTML page is split into two parts. The **head** and the **body**.

The **head** contains important webpage information like the page title (the text in the browser tab), stylesheets, scripts and meta information.

The **body** contains webpage content that is visible to the user.


## Let's get coding!

Let's start by defining the basic structure of your website. Create a new folder for your work called "HTML tutorial 1". Then inside this folder create a new file called "index.html". 

Using what we just learnt, and with guidance from your coach, create the following: 

* declare the doctype to be HTML
* open and close a set of `<html></html>` tags
* Within this, create the head and body tags

> If you load this in your browser, do you see anything on the page?

Now inside your head tag create a `<title>` tag with **My Inspirations** as your title.

> You should see that the tab bar has changed. If not, double check your code.

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My Inspirations</title>
  </head>
  <body>
  </body>
</html>
```

Notice how each tag is indented to its parent tag. This is important as it makes your code much easier to read and you'll be able to see nested tags much easier.

### Element: Headings 

Headings come in 6 sizes

# `<h1>Heading</h1>`
## `<h2>Heading</h2>`
### `<h3>Heading</h3>`
#### `<h4>Heading</h4>`
##### `<h5>Heading</h5>`
###### `<h6>Heading</h6>`

A `h1` defines the most important heading whereas a `h6` defines the least important.

Add a `h1` heading tag with the text "Beyonce Knowles" inside the body tag of your page.

### Element: Paragraph `<p>`

Putting content into a `<p>` tag will break your text up into paragraphs. This helps make the content of your page easier to read for the user.

Add an intro paragraph about your subject inside your `<body>` tag, after the `<h1>`:

```html
<p>
  Beyoncé Giselle Knowles-Carter (born September 4,
  1981) is an American singer, songwriter, record producer and actress.
  Born and raised in Houston, Texas, she performed in various singing and dancing
  competitions as a child and rose to fame in the late 1990s as lead singer of
  R&B girl-group Destiny's Child.
</p>
```

### Element: Link `<a>`

A link lets the user click through to another webpage. We use the attribute `href` to indicate where you want the user to go.

Let's add a link at the end of the paragraph:

```html
<a href="http://beyonce.com">Official Website</a>
```

### Element: Div `<div>`

A `div` tag lets you group elements together. Grouping elements is useful as we can later style them together (e.g. giving them all the same colour).

Wrap your existing paragraph and link in a div and add a new heading to it.

```html
<div>
  <h1>Beyonce Knowles</h1>
  <p>
    Beyoncé Giselle Knowles-Carter (born September 4,
    1981) is an American singer, songwriter, record producer and actress.
    Born and raised in Houston, Texas, she performed in various singing and dancing
    competitions as a child and rose to fame in the late 1990s as lead singer of
    R&B girl-group Destiny's Child.
    <a href="http://beyonce.com">Official Website</a>
  </p>
</div>
```

### Element: List `<li>`

There are two types of lists that can included on a webpage, **ordered** and **unordered**.
An unordered list `<ul>` is defined with bullets whilst an ordered list `<ol>` uses a numbered sequence.

Let's create a new `<h2>` then underneath list the reasons why this person
inspires us:

```html
<h2>Reasons why Beyonce inspires me</h2>
<ol>
  <li>She is one of the most successful female soloists in history</li>
  <li>She uses her art to call out social and political injustice</li>
  <li>She is a positive role model for young women and men</li>
</ol>
```

> If you wanted to make this an unordered list, what would you change? How could you check it worked? Try it, then change your list back to an ordered list.

### Element: Image `<img>`

So far we've learned a lot about how to add text to our page. Now let's add some images!

Before we start, we'll need to add the image files we want to use to the project folder.  It's very important to keep images in their own folder, so first, create a folder called 'images' inside the same folder as your HTML file.  Next, download at least five images of your subject to this folder. To do this, right-click on the image, click 'Save Image As', navigate to your /images directory, and save the image there. For this tutorial, we've named them 'img01.jpg', 'img02.jpg' and so forth, but feel free to use different filenames and change your code accordingly!

Images are primarily made up of three attributes

* the `<img>` tag
* the `src` attribute, which lets the page know what image we want to view
* the `alt` attribute, this provides extra information if the image cannot be seen on the webpage for any reason

In order for us to see this image on the webpage we need to link to the image, this involves telling the webpage where it is and what it is called. Before the main heading of the page, add the following

```html
<div>
  <img src="images/img01.jpg" alt="Beyonce">
</div>
```

Here you can see we have told the `src` of the image to look in the images folder and display the image `logo.png`, then we have given it a relevant `alt` attribute.

Let's add some more images. This time, we'll put them in a list.

Do this underneath the `<h2>Reasons why Beyonce inspires me</h2>` heading.

```html
<ul>
  <li><img src="images/img01.jpg" alt="portrait"></li>
  <li><img src="images/img02.jpg" alt="Super Bowl"></li>
  <li><img src="images/img03.jpg" alt="Lemonade"></li>
</ul>
```

## Adding a link on multiple elements

Links can contain many elements - not just text.

Let's use some pictures and text to link to a video. It can be handy when we want the user to get to where we want without needing to click on text.

Add this underneath the ordered list about why Beyonce is inspirational.

```html
<div>
  <a href="https://youtu.be/ZJRnLUI1EZ0?list=PLnHDtJ54PUGWUCaUoFWMZa9zkOLGxu8Pm">
    <img src="images/img04.jpg" alt="Link to video">
    <br/>
    Watch the Lemonade video
  </a>
</div>
```

> Click any of the images. Can you get to the link's page?
> What happens if you take the `<br/>` tag out? Remember to put it back afterwards!

If you have more images, add them into your page anywhere you like.

## Formatting text

We can also **emphasise** or make text *important*.
For emphasis we use `<strong>` and for importance `<em>`

Let's add a new paragraph after the first one and emphasise some of the content.

```html
<p>
  Beyoncé has stated that she is personally inspired by US First Lady Michelle
  Obama, saying <strong>"She proves you can do it all"</strong> and she has described Oprah
  Winfrey as <em>"the definition of inspiration and a strong woman"</em>.
</p>
```
### mailto links `<a>`

Links can also open up a user's email client and share content. The difference between links and mailto links is the content defined in the **href** attribute.

```html
<ul>
  <li>
     <a href="mailto:me@mywebsite.com?subject=I love Beyonce too!">Email me</a>
  </li>
  <li>
     <a href="mailto:?subject=I love Beyonce too!">Email a friend</a>
  </li>
</ul>
```

> What happens when you click the first link?

> What happens when you click the second link? How is it different?

> What happens when you add `&body=Beyonce is amazing` to the second link?

### Commenting

You can use a special kind of tag to add notes to our page that the computer will ignore. Comments are particularly useful when wanting to remind yourself, or other programmers, how your code works.

```html
<!-- Note to self: this is where the header goes -->
```

## Bonus

### Twitter share 

Add a share on twitter link along with your other sharing links.

```html
<a href="http://twitter.com/home?status=I just build my first webpage at Coders of Colour">Share your work on twitter</a>
```
-----
This ends our first lesson, we hope you enjoyed it and learnt something. If you have some spare time how about going back through this tutorial and, by yourself, make some amendments.

## Further resources

* [Codecademy Interactive HTML Tutorial](https://www.codecademy.com/learn/web)
* [HTML elements](https://developer.mozilla.org/en/docs/Web/HTML/Element)
* [Special characters](http://htmlandcssbook.com/extras/html-escape-codes)
* [The Bare Bones Guide to HTML](http://werbach.com/barebones/barebones.html)

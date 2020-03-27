---
id: Basic_HTML_and_HTML5
title: Basic HTML and HTML5
sidebar_label: Basic HTML and HTML5
---

## Introduction to HTML5 Elements

HTML5 introduces more descriptive tags like header, footer, nav, video, article, section and others.

```html
<!DOCTYPE html>
<html>
  <head>
  </head>
  <body>
    <p>I'm a paragraph</p>
  </body>
</html>
```

## HTML Semantic Elements

HTML Semantic Elements
Websites often display content in multiple columns (like a magazine or newspaper).

```html
<header> - Defines a header for a document or a section
<nav> - Defines a container for navigation links
<section> - Defines a section in a document
<article> - Defines an independent self-contained article
<aside> - Defines content aside from the content (like a sidebar)
<footer> - Defines a footer for a document or a section
<details> - Defines additional details
<summary> - Defines a heading for the <details> element
```

## Add Images to Your Website

To add image

```html
<img src="https://bit.ly/fcc-relaxing-cat" alt="Author standing on a beach with two thumbs up.">
```

Notes:

- img elements are self-closing.
- All img elements must have an alt attribute.
- Alt attribute is used for screen readers to improve accessibility and is displayed if the image fails to load.
- If the image is purely decorative, using an empty alt attribute is a best practice.

## Link to External Pages with Anchor Elements

Anchor elements need a destination web address called an href attribute. They also need anchor text. Here's an example:

```html
<a href="http://freecatphotoapp.com">
<img src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back.">
</a>
```

## Link to Internal Sections of a Page with Anchor Elements

Assign the href to a id
An id is an attribute that uniquely describes an element.

```html
<a href="#contacts-header">Contacts</a>
...
<h2 id="contacts-header">Contacts</h2>
```

## Nest an Anchor Element within a Paragraph

Example

<p>
Here's a <a target="_blank" href="http://freecodecamp.org"> link to freecodecamp.org</a> for you to follow.
</p>
In code:

```html
<p>
Here's a <a target="_blank" href="http://freecodecamp.org">
 link to freecodecamp.org</a> for you to follow.
</p>
```

## Make Dead Links Using the Hash Symbol

Sometimes you want to add a elements to your website before you know where they will link.

This is also handy when you're changing the behavior of a link using JavaScript

```html
<p>Click here to view more <a href="#" target="_blank">cat photos</a>.</p>
```

## Turn an Image into a Link

```html
<a href="#"><img src="https://bit.ly/fcc-running-cats" alt="Three kittens running towards the camera."></a>
```

## Create a Bulleted Unordered List

```html
<ul>
  <li>milk</li>
  <li>cheese</li>
</ul>
```

## Create an Ordered List

```html
<ol>
  <li>Garfield</li>
  <li>Sylvester</li>
</ol>
```

## Create a Text Field

Inputs are self closing

```html
<input type="text">
```

## Add Placeholder Text to a Text Field

```html
<input type="text" placeholder="this is placeholder text">
```

## Create a Form Element

```html
<form action="/url-where-you-want-to-submit-form-data"></form>
```

## Add a Submit Button to a Form

```html
<button type="submit">this button submits the form</button>
```

## Use HTML5 to Require a Field

```html
<input type="text" placeholder="cat photo URL" required>
```

## Create a Set of Radio Buttons

- Same Name - All related radio buttons should have the same name attribute to create a radio button group.
- For Label - It is considered best practice to set a for attribute on the label element, with a value that matches the value of the id attribute of the input element. This allows assistive technologies to create a linked relationship between the label and the child input element.

```html
<label for="indoor">
  <input id="indoor" type="radio" name="indoor-outdoor">Indoor
</label>
```

## Create a Set of Checkboxes

```html
<label for="loving">
  <input id="loving" type="checkbox" name="personality"> Loving
</label>
```

## Check Radio Buttons and Checkboxes by Default

> You can set a checkbox or radio button to be checked by default using the checked attribute.

```html
<input type="radio" name="test-name" checked>
```

## Nest Many Elements within a Single div Element

> The div element, also known as a division element, is a general purpose container for other elements.

```html
<div>
  <p>Things cats love:</p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  </div>
```

## Declare the Doctype of an HTML Document

> The ! and uppercase DOCTYPE is important, especially for older browsers. The html is not case sensitive.

```html
<!DOCTYPE html>
<html>
  <!-- Your HTML code goes here -->
</html>
```

## Define the Head and Body of an HTML Document

> Metadata elements, such as link, meta, title, and style, typically go inside the head element.

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- metadata elements -->
  </head>
  <body>
    <!-- page contents -->
  </body>
</html>
```

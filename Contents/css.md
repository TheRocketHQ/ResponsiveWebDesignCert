---
id: Basic_CSS
title: Basic CSS
sidebar_label: Basic CSS
---

## Change the Color of Text

> Note that it is a good practice to end inline style declarations with a ; .

```html
<h2 style="color: blue;">CatPhotoApp</h2>
```

## Use CSS Selectors to Style Elements

-   You should have both { }
-   Be sure to add a semicolon to the end of each of your element's style rules.

```html
<style>
  h2 {color: red;}
</style>
```

## Use a CSS Class to Style an Element

-   in your CSS style element, class names start with a period
-   HTML elements' class attribute, the class name does not include the period.

```html
<style>
  .blue-text {
    color: blue;
  }
</style>
```

## Style Multiple Elements with a CSS Class

-   Classes are meant to be used on several elements

```html
...
    <h2 class="red-text">CatPhotoApp</h2>
    <main>
      <p class="red-text">Click here to view more <a href="#">cat photos</a>.</p>
...
```

## Change the Font Size of an Element

Example of setting the font size of a h1 to 30px; Be aware that font size can take several values besides pixels this is just an example

```css
h1 {
	font-size: 30px;
}
```

## Set the Font Family of an Element

```css
h2 {
	font-family: sans-serif;
}
```

## Import a Google Font

1. Import the link above the style
2. Use the desired font - font-family: FAMILY_NAME, GENERIC_NAME;

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
    h2 {
        font-family: Lobster;
    }
</style>
```

## Specify How Fonts Should Degrade

In case the desired font won't load: Helvetica > sans-serif...

```css
p {
	font-family: Helvetica, sans-serif;
}
```

## Size Your Images

```css
.larger-image {
	width: 500px;
}
```

## Add Borders Around Your Elements

```css
.thin-red-border {
	border-color: red;
	border-width: 5px;
	border-style: solid;
}
```

## Add Rounded Corners with border-radius

Use border Radius

```css
.thick-green-border {
	border-color: green;
	border-width: 10px;
	border-style: solid;
	border-radius: 10px;
}
```

## Make Circular Images with a border-radius

border-radius: 50%;

```css
.thick-green-border {
	border-color: green;
	border-width: 10px;
	border-style: solid;
	border-radius: 50%;
}
```

## Give a Background Color to an Element

```css
.green-background {
	background-color: green;
}
```

## Set the id of an Element

-   ID's are meant to be unique

```html
<h2 id="cat-photo-app">
```

## Use an id Attribute to Style an Element

```css
#cat-photo-element {
	background-color: green;
}
```

## Adjust the Padding of an Element

Padding is the inside space from the content to it's borders

```css
#cat-photo-element {
	background-color: green;
	padding: 20 px;
}
```

## Adjust the Margin of an Element

Margin is the Outise space from the it's borders towards the next or parent content

```css
#cat-photo-element {
	background-color: green;
	margin: 20 px;
}
```

## Add a Negative Margin to an Element

> An element's margin controls the amount of space between an element's border and surrounding elements. If you set an element's margin to a negative value, the element will grow larger.

## Add Different Padding to Each Side of an Element

> CSS allows you to control the padding of all four individual sides of an element with the padding-top, padding-right, padding-bottom, and padding-left properties.

```css
#cat-photo-element {
	padding: top, right, bottom, left;
}
```

## Add Different Margins to Each Side of an Element

## Use Clockwise Notation to Specify the Padding of an Element

## Use Clockwise Notation to Specify the Margin of an Element

## Use Attribute Selectors to Style Elements

## Understand Absolute versus Relative Units

## Style the HTML Body Element

## Inherit Styles from the Body Element

## Prioritize One Style Over Another

## Override Styles in Subsequent CSS

## Override Class Declarations by Styling ID Attributes

## Override Class Declarations with Inline Styles

## Override All Other Styles by using Important

## Use Hex Code for Specific Colors

## Use Hex Code to Mix Colors

## Use Abbreviated Hex Code

## Use RGB values to Color Elements

## Use RGB to Mix Colors

## Use CSS Variables to change several elements at once

## Create a custom CSS Variable

## Use a custom CSS Variable

## Attach a Fallback value to a CSS Variable

## Cascading CSS variables

## Change a variable for a specific area

## Use a media query to change a variable

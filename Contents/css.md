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

Sometimes you will want to customize an element so that it has a different `margin`on each of its sides.

CSS allows you to control the `margin`of all four individual sides of an element with the `margin-top`, `margin-right`, `margin-bottom`, and `margin-left`properties.  

## Use Clockwise Notation to Specify the Padding of an Element

Instead of specifying an element's `padding-top`, `padding-right`, `padding-bottom`, and `padding-left`properties individually, you can specify them all in one line, like this:

```css
padding: 10px 20px 10px 20px;
```

These four values work like a clock: top, right, bottom, left, and will produce the exact same result as using the side-specific padding instructions.

## Use Clockwise Notation to Specify the Margin of an Element

Instead of specifying an element's `margin-top`, `margin-right`, `margin-bottom`, and `margin-left`properties individually, you can specify them all in one line, like this:

```css
margin: 10px 20px 10px 20px;
```

These four values work like a clock: top, right, bottom, left, and will produce the exact same result as using the side-specific margin instructions.

## Use Attribute Selectors to Style Elements

You have been giving `id`or `class`attributes to elements that you wish to specifically style. These are known as ID and class selectors. There are other CSS Selectors you can use to select custom groups of elements to style.

Let's bring out CatPhotoApp again to practice using CSS Selectors.

For this challenge, you will use the `[attr=value]`attribute selector to style the checkboxes in CatPhotoApp. This selector matches and styles elements with a specific attribute value. For example, the below code changes the margins of all elements with the attribute `type`and a corresponding value of `radio`:

```css
[type='radio'] {
  margin: 20px 0px 20px 0px;
}
```

## Understand Absolute versus Relative Units

The last several challenges all set an element's margin or padding with pixels \(`px`\). Pixels are a type of length unit, which is what tells the browser how to size or space an item. In addition to `px`, CSS has a number of different length unit options that you can use.

The two main types of length units are absolute and relative. Absolute units tie to physical units of length. For example, `in`and `mm`refer to inches and millimeters, respectively. Absolute length units approximate the actual measurement on a screen, but there are some differences depending on a screen's resolution.

Relative units, such as `em`or `rem`, are relative to another length value. For example, `em`is based on the size of an element's font. If you use it to set the `font-size`property itself, it's relative to the parent's `font-size`.

**Note**  
There are several relative unit options that are tied to the size of the viewport. They are covered in the Responsive Web Design Principles section.

## Style the HTML Body Element

Every HTML page has a `body`element.

We can prove that the `body`element exists here by giving it a `background-color`of black.

We can do this by adding the following to our `style`element:

```css
body {
  background-color: black;
}
```

## Inherit Styles from the Body Element

Now we've proven that every HTML page has a `body`element, and that its `body`element can also be styled with CSS.

Remember, you can style your `body`element just like any other HTML element, and all your other elements will inherit your `body`element's styles.

## Prioritize One Style Over Another

Sometimes your HTML elements will receive multiple styles that conflict with one another.

For example, your `h1`element can't be both green and pink at the same time.

Let's see what happens when we create a class that makes text pink, then apply it to an element. Will our class _override_ the `body`element's `color: green;`CSS property?

## Override Styles in Subsequent CSS

Our "pink-text" class overrode our `body`element's CSS declaration!

We just proved that our classes will override the `body`element's CSS. So the next logical question is, what can we do to override our `pink-text`class?

## Override Class Declarations by Styling ID Attributes

We just proved that browsers read CSS from top to bottom. That means that, in the event of a conflict, the browser will use whichever CSS declaration came last.

But we're not done yet. There are other ways that you can override CSS. Do you remember id attributes?

Let's override your `pink-text`and `blue-text`classes, and make your `h1`element orange, by giving the `h1`element an id and then styling that id.

## Override Class Declarations with Inline Styles

So we've proven that id declarations override class declarations, regardless of where they are declared in your `style`element CSS.

There are other ways that you can override CSS. Do you remember inline styles?

## Override All Other Styles by using Important

Yay! We just proved that inline styles will override all the CSS declarations in your `style`element.

But wait. There's one last way to override CSS. This is the most powerful method of all. But before we do it, let's talk about why you would ever want to override CSS.

In many situations, you will use CSS libraries. These may accidentally override your own CSS. So when you absolutely need to be sure that an element has specific CSS, you can use `!important`

Let's go all the way back to our `pink-text`class declaration. Remember that our `pink-text`class was overridden by subsequent class declarations, id declarations, and inline styles.

## Use Hex Code for Specific Colors

Did you know there are other ways to represent colors in CSS? One of these ways is called hexadecimal code, or `hex code`for short.

We usually use `decimals`, or base 10 numbers, which use the symbols 0 to 9 for each digit. `Hexadecimals`\(or `hex`\) are base 16 numbers. This means it uses sixteen distinct symbols. Like decimals, the symbols 0-9 represent the values zero to nine. Then A,B,C,D,E,F represent the values ten to fifteen. Altogether, 0 to F can represent a digit in `hexadecimal`, giving us 16 total possible values. You can find more information about [hexadecimal numbers here](https://en.wikipedia.org/wiki/Hexadecimal).

In CSS, we can use 6 hexadecimal digits to represent colors, two each for the red \(R\), green \(G\), and blue \(B\) components. For example, `#000000`is black and is also the lowest possible value. You can find more information about the [RGB color system here](https://en.wikipedia.org/wiki/RGB_color_model).

```css
body {
  color: #000000;
}
```

## Use Hex Code to Mix Colors

To review, hex codes use 6 hexadecimal digits to represent colors, two each for red \(R\), green \(G\), and blue \(B\) components.

From these three pure colors \(red, green, and blue\), we can vary the amounts of each to create over 16 million other colors!

For example, orange is pure red, mixed with some green, and no blue. In hex code, this translates to being `#FFA500`.

The digit `0`is the lowest number in hex code, and represents a complete absence of color.

The digit `F`is the highest number in hex code, and represents the maximum possible brightness.

## Use Abbreviated Hex Code

Many people feel overwhelmed by the possibilities of more than 16 million colors. And it's difficult to remember hex code. Fortunately, you can shorten it.

For example, red's hex code `#FF0000`can be shortened to `#F00`. This shortened form gives one digit for red, one digit for green, and one digit for blue.

This reduces the total number of possible colors to around 4,000. But browsers will interpret `#FF0000`and `#F00`as exactly the same color.

## Use RGB values to Color Elements

Another way you can represent colors in CSS is by using `RGB`values.

The RGB value for black looks like this:

`rgb(0, 0, 0)`

The RGB value for white looks like this:

`rgb(255, 255, 255)`

Instead of using six hexadecimal digits like you do with hex code, with `RGB`you specify the brightness of each color with a number between 0 and 255.

If you do the math, the two digits for one color equal 16 times 16, which gives us 256 total values. So `RGB`, which starts counting from zero, has the exact same number of possible values as hex code.

Here's an example of how you'd change the body background to orange using its RGB code.

```css
body {
  background-color: rgb(255, 165, 0);
}
```

## Use RGB to Mix Colors

Just like with hex code, you can mix colors in RGB by using combinations of different values.

Replace the hex codes in our `style`element with their correct RGB values.

| Color  | RGB                  |
| :----- | :------------------- |
| Blue   | `rgb(0, 0, 255)`     |
| Red    | `rgb(255, 0, 0)`     |
| Orchid | `rgb(218, 112, 214)` |
| Sienna | `rgb(160, 82, 45)`   |

## Use CSS Variables to change several elements at once

CSS Variables are a powerful way to change many CSS style properties at once by changing only one value.

Follow the instructions below to see how changing just three values can change the styling of many elements.

## Create a custom CSS Variable

After you create your variable, you can assign its value to other CSS properties by referencing the name you gave it.

```css
background: var(--penguin-skin);
```

This will change the background of whatever element you are targeting to gray because that is the value of the `--penguin-skin`variable.

Note that styles will not be applied unless the variable names are an exact match.

## Use a custom CSS Variable

After you create your variable, you can assign its value to other CSS properties by referencing the name you gave it.

```css
background: var(--penguin-skin);
```

This will change the background of whatever element you are targeting to gray because that is the value of the `--penguin-skin`variable.

Note that styles will not be applied unless the variable names are an exact match.

## Attach a Fallback value to a CSS Variable

When using your variable as a CSS property value, you can attach a fallback value that your browser will revert to if the given variable is invalid.

**Note:** This fallback is not used to increase browser compatibilty, and it will not work on IE browsers. Rather, it is used so that the browser has a color to display if it cannot find your variable.

Here's how you do it:

```css
background: var(--penguin-skin, black);
```

This will set background to black if your variable wasn't set.

**Note** that this can be useful for debugging.  

## Cascading CSS variables

When you create a variable, it becomes available for you to use inside the element in which you create it. It also becomes available within any elements nested within it. This effect is known as cascading.

Because of cascading, CSS variables are often defined in the :rootelement.

You can think of the `:root`element as a container for your entire HTML document, in the same way that an `html`element is a container for the `body`element.

By creating your variables in `:root`, they will be available throughout the whole web page.  

## Change a variable for a specific area

When you create your variables in `:root`they will set the value of that variable for the whole page.

You can then over-write these variables by setting them again within a specific element.

## Use a media query to change a variable

CSS Variables can simplify the way you use media queries.

For instance, when your screen is smaller or larger than your media query break point, you can change the value of a variable, and it will apply its style wherever it is used.

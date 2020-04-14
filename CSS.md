# CSS
## Definition
> CSS stands for Cascading Style Sheet, We can change almost anything, font, colours and layouts

> Its best to write CSS in an external style sheet, we make one by just adding a .css at the end of it

> TO tell the HTML page we are using a style sheet and where to look we use a link tag. The < head> of the HTML document is where we put information that our browser needs in order to render the page properly

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <link rel="stylesheet" href="/styles.css">
  <title>My Awesome Web Page</title>
</head>
<body>

</body>
</html>
```

### Link Tag

```html
<link rel="stylesheet" href="/styles.css">
```
> There are two attributes here, rel and href
* rel: relationship between current document and the linked document/resource
* href: the location of the linked document

> We're linking a stylesheet and here is where you can find it

### Anatomy of a CSS block

Three Parts:

1. Selector: Which elements we want to style 
2. Property: What about those elements do we need to change
3. Value: What do we want to change it to 

![alt text](https://github.com/ShivamP96/HTML-and-CSS-Essentials/blob/master/pictures/CSSstructure.png "CSS Structure")


---
## Selectors, Classes & IDs

> Selectors allow us to pick an element, we can do this using **tags**, **classes** or **id's**

> Below are examples using all 3 methods

### HTML Tags (just put the letter)

```html
<h1> Our Awesome Page </h1>

<p> The first paragraph </p>
<p> The second paragraph </p>
```
#### CSS
>Turns all the paragraph tags purple
```css
p {
  color: purple;
}
```

### Classes (.classname)
> Classes are an example of HTML attributes (little pieces of information we can add to HTML tags).
>  We use classes when we want to share the styles between more than one HTML Tag. One tag can have as many classes as we want, and a class can be used as many times as you'd like on a web page. 

```html
<h1 class="highlight"> My First Blog Post </h1>

<p> The first paragraph of my awesome blog post </p>

<p class="highlight"> The second paragraph </p>
```

#### CSS
see how we use .classname thats syntax for classes
```css
.highlight {
  color: yellow;
}
```

> This code would make the h1 and second paragraph font yellow

### ID's
> When you want to style one unqiue element on the page. Each HTML element can only have one ID, and each ID on your webpage has to be unique. Alerts and notifications are a great example of when you might want to use an ID. 

```HTML
<p id="alert"></p>
```

#### CSS
we use  # for ID's 
```css
#alert {
  background-color: red;
}
```
---

## Fonts
> If we want to use Arial on our webpage, we can select the body tag and the font-family property to change the font of all our element

sans-serif is the fallback in the event that Arial doesn't work

```css
body {
  font-family: Arial, sans-serif
}
```
### Custom Fonts 
We can go to google fonts and grab one from there and they give you a code snippit to add to your code

[Google Fonts](https://fonts.google.com/)



### We can style fonts even further using a variety of different properties


#### Font-style

can be set to: normal, italic, oblique

```css
p {
  font-style: italic;
}
```
#### Font-weight
style without using < strong>. Normal, bold, bolder, lighter, or a number from 100 to 900 (numbers must be multiple of 100)

```css
p {
  font-weight: bold;
}
```

#### Font-size 
using h1-h6 tags can give us different sized fonts, but if you wanna be a bit more specific

```css
.blog-title {
  font-size: 30px;
}
```

#### Text-align
Sets the alignment of the text -left, right center or justify

```css
p {
  text-align: center;
}
```

#### Text-transform
Allows you to make all of our text uppercase or lowercase. Takes the properties: capitalize, uppercase, lowercase

```css
#alert {
  text-transform: uppercase;
}
```

#### Letter-spacing
Sets the space between letters. Can be set to negative numbers

```css
p {
  letter-spacing: 10px;
}
```
---

## Colours 🌈

> List of built in colour names found here
[color list](https://www.w3schools.com/cssref/css_colors.asp)

**Colour is spelt the American way without the U**

```css
h1 {
  color: tomato;
  background-color: blue;
}
```
### Hexadecimal Colours

> You can make any colour by combining red, yellow, and blue. 

[Css Hex]()





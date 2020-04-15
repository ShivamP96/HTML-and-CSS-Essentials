# HTML Notes

### Definition
> **HTML** stands for *"Hyper Text Markup Language"*. It gives us a way to *'markup'* our text so that the browser can understand. Its made up of tags, each tag has its own default styles that we can override. 

>Each HTML element is made up of three basic pieces: 
> 1. An opening tag 
> 2. Some content
> 3. Closing tag
---
### Structure

``` javascript 
Opening Tag -- [ <p> ]
Content ------ [ I'm a paragraph ]
Closing Tag ---[ </p> ]

```
---
### Attributes
> When our HTML tags ^ needs more info we add something called attributes. 
> They are always added to the **Opening** HTML tag e.g. class, href etc...
```
<p class="highlights"> 
  I'm a paragraph
</p>
 ```

| Attribute Name  | Attribute Value  |
| :--------------:| :--------------: |
|   "Class"       |  "highlights"    |
|   "href"        | "http://google.ca"|

> Hint: Google the HTML tags you don't know 

---

### Image Tags
 >Image tags are self closing, they don't need a closing tag. 

 >The image tag requires two pieces of information:
> 1.  **src** (source) : Tells the tag where it can find the image we want to display
> 
> 2.  **alt** : Is read by screen readers and shown if the image doesn't load proeprly.... **Always include this**

``` html
Reminder: Always add HTML attributes to the opening tags, with self closing tags, we add them to the only HTML Tag

Example: 
<img src="http://somecat.com/g/403" alt="super cute kitten">

    Self Closing Tag

```
---
### Text Tags
> Ready made HTML tags to help you organize all of the content on your page
> CSS will be used to tweak these tags

#### Headings
> They describe the hierarchy of information on your web page. They can be used to make the topics on  your web page more obvious and search engines can locate them. 

``` html

<h1>I'm an h1</h1>
<h2>I'm an h2</h2>
<h3>I'm an h3</h3>
<h4>I'm an h4</h4>
<h5>I'm an h5</h5>
<h6>I'm an h6</h6>
```
<h1>I'm an h1</h1>
<h2>I'm an h2</h2>
<h3>I'm an h3</h3>
<h4>I'm an h4</h4>
<h5>I'm an h5</h5>
<h6>I'm an h6</h6>

#### Paragraphs
> One of the most used HTML tags is the paragraph tag

``` html
<p>I'm a paragraph </p>
```
> Each paragraph tag has spaces around it so you can use it to easily wrap individual paragraphs

#### Bold and Italics in Paragraph Tags
> We can use the < Strong > and < em > tags respectively

```html
<p>Let's get a little bit <strong>bold</strong></p>
```
<p> Let's get a little bit <strong>bold</strong></p>

```html
<p> Or we can try <em>italics</em></p>
```
<p> Or we can try <em>italics</em></p>

> Hint: You have to nest them accordingly, check below and see how they are all inner and outer paired. The em opens and closes, the strong tag doesn't close first.

```html
<p> Or we can have text that's both <strong><em>italic and bold </em></strong></p>
```
<p> Or we can have text that's both <strong><em>italic and bold </em></strong></p>

---
### Lists
> HTML has an element for creating lists
##### Structure
> 1. Parent tags that describes the type of list
> 2. Child List elements

#### Ordered Lists
> We use < ol > and add things by using < li >

```html
<h4>Chocolate Chip Cookies </h4>
<ol>
  <li>Preheat oven to 350</li>
  <li>Mix sugar, butter, vanilla and egg in a large bowl</li>
  <li>Mix baking soda, flour and salt together </li>
</ol>
```

<h4>Chocolate Chip Cookies </h4>
<ol>
  <li>Preheat oven to 350</li>
  <li>Mix sugar, butter, vanilla and egg in a large bowl</li>
  <li>Mix baking soda, flour and salt together </li>
</ol>

#### Unordered List
> we use < ul > and add things by using < li > again, see how easy this is!!!

```html
<ul>
  <li>1 teaspoon vanilla</li>
  <li>1 egg</li>
  <li>3/4 cup brown sugar</li>
</ul>
```

<ul>
  <li>1 teaspoon vanilla</li>
  <li>1 egg</li>
  <li>3/4 cup brown sugar</li>
</ul>

#### Description List
> If you have to define something like a glossary of terms or something like that

> There is one parent tag: < dl > = description list
> Two child tags: 
> 1. < dt > = defines a term in the description list
> 2. < dd > = defins the description of that term

```html
<dl>
  <dt>Pizza</dt>
  <dd>a dish of Italian origin consisting of a flat, round base of dough baked with a topping of tomato sauce and cheese, typically with added meat or vegetables.</dd>

  <dt>Coffee</dt>
  <dd>a drink made from the roasted and ground bean-like seeds of a tropical shrub, served hot or iced.</dd>

</dl>
```

<dl>
  <dt>Pizza</dt>
  <dd>a dish of Italian origin consisting of a flat, round base of dough baked with a topping of tomato sauce and cheese, typically with added meat or vegetables.</dd>

  <dt>Coffee</dt>
  <dd>a drink made from the roasted and ground bean-like seeds of a tropical shrub, served hot or iced.</dd>

</dl>

---
### Links
> This is how we navigate around the web, like an image tag they need an attribute called href

> We use the anchor tag < a > to make a link
>. href stands for <strong>hypertext reference</strong>. It tells the anchor tag where to go once its been clicked. 

```html
<a href="https://google.ca">Go to Google </a>
```
<a href="https://google.ca">Go to Google </a>

#### Target Attribute
> we can add another attribute ontop of the href attribute to do special things.

##### New Tab
> We can add a new attribute, target, to our link tag if we want our link to open up in a new tab.

```html
<a href="https://google.ca" target="_blank">Go to Google, but in a new tab </a>
```

<a href="https://google.ca" target="_blank">Go to Google, but in a new tab </a>

#### Email
> Always wondered why you can click a link and it'll open up the email link as well

```html
<a href="mailto:hell@gmail.com"> Email Me! </a>
```
> The email address will already be filled in for you

<a href="mailto:hell@gmail.com"> Email Me! </a>

#### Phone Number
> Now we can call people with the click of a button
```html
<a href="tel:1-555-555-5555">Call Me! </a>
```
<a href="tel:1-555-555-5555">Call Me! </a>


### More about href
> The href attribute takes two different kinds of paths, <strong>absolute</strong> and <strong>relative</strong>. So far, we've just been using absolute paths. 

>Absolute paths start with http:// or https:// you can think of them like directions you could follow no matter where you started.

> A relative path on the other hand, is telling your file where to find another page, based on where they're located.

```html
project 
  /view
    index.html
    about.html
  /styles
    styles.css
```
 Lets add a link to the about page 

```html
<a href="./about.html"> About Us! </a>
```
You see how that works, we used a " ./ " to look in the current directory

Here is another example but us looking at a relative path outside of our folder structure

```html
project 
  /views 
    index.html 
    about.html 
  /users
    profile.html
  /styles 
    styles.css   
```
How would we link to the profile page???

```html
<a href="../users/profile.html"> About us </a>
```
---

## Structure of our pages

> There are HTML Tags that help us organize our web pages otherise we will just have everything in a < div > and it'll be hard to find out where things are

> The following is a list of semantic tags that have meaning and help us organize our code

```html
<article>
<aside>
<main>
<nav>
<section>
<header>
<footer>
<div>
```

#### Basic code needed to build a webpage

<ul>
  <li> < head> is where we put any information the browser needs in oder to render the page properly
  <li> Only the title tag is displayed to the user, the rest is hidden
  <li> Body tag is where you write all the code that the users will see
</ul>


```html
Example 1
<!DOCTYPE html>
<html>
<head>
  <title>Document</title>
</head>
<body>


</body>
</html>
```

```html
Example 2 ( header, main, sidebar and footer)
<!DOCTYPE html>
<html>
<head>
  <title>Document</title>
</head>
<body>
  <header>
    <h1> Title Of the Webpage </h1>
  </header>
  <aside>
    <ul>
      <li> Home Page </li>
    </ul>
  </aside>
  <main>
    <p> I'm the main section of the page </p>
  </main>
  <footer>
    Footer Content!
  </footer>
</body>
</html>

```



---

### Div

Already adds its own < br/> so you don't need a line break 

if you use a span its used for inline and small elemental changes

otherwise use a div

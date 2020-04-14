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

![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")
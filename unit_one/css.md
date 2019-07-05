![Cascading Style Sheets refers to the manner in which styles grabbed from files that containg styling information are blanketed across a page and ordered by their specificity](./images/cssHeader1.jpg)

### 3 METHODS OF APPLYING CSS

***Inline***: Inline CSS styles are written into an HTML tag. 

` <p style="color: blue;">`

***Internal***: Internal css is written inside of an HTML document, inside the `<head>` tag, between two `<style>` tags. 
``` 
<style>
p {
    color: blue;
  }
</style> 
```

***External***: Seperate CSS files that are linked into the head of an HTML document are known as external css.

```
<head>
  <link rel="stylesheet" href="./style.css> 
</head>
``` 

### SELECTORS

This is either the tag we are trying to effect, or a special "name" that we give an html element in the form of an *ID* or a *class*. 

***Element Selectors***: These select the HTML elements with a matching HTML tag. This is the LEAST SPECIFIC CSS rule. 
``` 
p {
    background-color: black;
}

div {
    background-color: yellow
}
```

***Class Selectors***: These select those HTML elements with a matching class attribute. *They are prepended by a period*

index.html
```
<img class="small-image" src="www.someurl.com">
```

style.css
```
.small-image {
    width: 100px;
}
```

***ID Selectors***: Refers to the element with a matching ID attribute. Unlike classes, which can be shared, IDs are *unique*. *They are prepended by a hashtag.*

index.html
``` 
<span id="bold-and-red">
```

style.css
```
#bold-and-red {
    font-weight: bold;
    color: red;
}
```

### SPECIFICITY

The order in which the browser decides to display styles. The most specific styles override the least. In this case, an ID's style will override a class's style, a class's style will override a tag's style. 

When we chain selectors, we increase the specificity of that style. 

##### CHAINING SELECTORS

If a specific HTML element has 2 or more selectors, one can refer to it like so: 

``` 
div.blue {
    background-color: blue;
}
```

In this example we are selecting the tag (div) with a class of blue.

##### MULTIPLE

To avoid redundancy, one can apply a style to multiple selectors separated by a comma. 

```
body, div, .class, #id {
    font-family: Batman Sans Serif;
}
```

##### !IMPORTANT

This special phrase, when included in a style, can override even an ID's style. It is technically the most specific rule. However, it's often recommended to avoid using !important as much as possible.

``` 
.anImportantStyle {
    color: tomato !important;
}
```
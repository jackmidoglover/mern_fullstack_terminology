![HTML stands for Hyper Text Markup Language, a computer language that defines the structure and presentation of raw text by surrounding that text with information the computer can process or "marking it up".](./images/htmlHeader.jpg "HTML header image")

### HTML ELEMENTS

An HTML element is a wrapper for content on a web page that contains information about the type and structure of the content nested within it that the computer can interpret. 


##### DOCUMENT TYPE DECLARATION 

A type of HTML element, usually the first in an HTML document, that instructs the browser about what type of language is being used in the document. 

``` 
<!DOCTYPE html>
``` 

##### TAGS

Elements wrapped in angle brackets that signify the structure of type of content. They often create hierarchical structures, that we speak about as ancestors. One tag or element can be the parent of another, which then becomes its child. That child can have its own child, which becomes the grandchild of its parent. 

Most come in pairs, with an "opening" or a "closing" tag. Some are self closing, like image tags.

``` 
<img />

<div> </div>

``` 

![Image of an HTML element, or a "unit" of content, with an opening tag, element content behind the opening tag, and a closing tag](./images/htmlElement.jpg "HTML element")


*** There are two special tags that define the page's content, the `<head>` tag and the `<body>` tag. The head tag stores meta data, or information that most people don't see (like links that the page might use for css.) The body contains the content that a user will see.

##### ATTRIBUTES 

Attributes in HTML are name-value pairs that provide information about an element's content, for example, "src", "alt" or "data-value". 

``` 
<img src="https://www.aprettypicture.com" alt="This is a pretty picture!" data-value="5" />
```



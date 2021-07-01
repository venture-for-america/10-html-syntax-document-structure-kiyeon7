# HTML Syntax & Document Structure

## Overview

In this lesson we will do a quick review of HTML syntax and document structure from the video lecture in the prior lesson.

## What's Covered in This Lesson

1. HTML Syntax
2. Document Structure

### Syntax

HTML stands for Hyper Text Markup Language. Markup languages surround content in order to tell the browser how to format it. HTML does this through a series of elements. HTML Elements are made up of a starting tag and an ending tag like so:

```html
<p>You're Learning HTML!</p>
```

Above we can see the `p` element which indicates a _paragraph_ to the browser. The start tag `<p>` indicates the beginning of the paragraph and the ending tag `</p>` defines the end of the paragraph. As you can see tags names are surrounded by `<>` angle brackets. All the content `You're Learning HTML!` in the center is the body of the paragraph. This tells the browser to add space before and after the content "You're Learning HTML!".

There are a few exceptions where elements may just have an opening tag only. We will see a few of these in examples below such as the image element `<img>` but more on that later.

Inside the starting tag `<p>` we can place attributes, such as `class="intro"` (in full, `<p class="intro">`), that help us refer to the paragraph element from JavaScript and CSS (more on that in a bit). These options are only found in the starting tag and never in the ending tag. We separate the element name `p` from the attribute name `class` using a keyboard space. We can set a value for our attribute `attribute="value"` using an `=` equals symbol and `"` quotes to surround our value.

### Document Structure

All HTML pages have a standardized document structure:

```html
<html>
  <head>
    <!-- Meta data for the browser and search engines -->
  </head>
  <body>
    <!-- Visible content area -->
  </body>
</html>
```

The `<html>` tag wraps all of the content and tells the browser that everything in between the starting and ending `<html>...</html>` tags is to be interpreted is HTML code. Nested inside `<html>...</html>`, we have the `<head>...</head>` and the `<body>...</body>`. The `head` contains data for the browser and search engines (such as the title of the page, links to other stylesheets and scripts, meta keywords, and descriptions, among others). This content is not something a visitor to our website will see directly.

In contrast, the `body` contains all of the visible content users see when they visit the webpage. This includes text such as headings, paragraphs, and images, links, videos, audio players, maps, forms, and more.

### Doctype

A special element proceeding the document structure is the `<!DOCTYPE>` tag.

```html
<!DOCTYPE html>
<html>
  <head>...</head>
  <body>...</body>
</html>
```

The Doctype tells the browser the version of HTML that it should interpret the document as. In the case of HTML5 you simply state `<!DOCTYPE html>`.

## Summary

- HTML elements wrap our content telling the browser how we wish to display things.
- HTML elements are written as `<start-tag>content</end-tag>`.
- HTML attributes can be added to the start tag `<start-tag attribute="value">`.
- HTMLs basic document structure is `<html><head>...</head><body>...</body></html>`.

# Resources

- [Mozilla Dev Network - Learn HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [HTML Element Lookup Reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)
- [HTML Element Cheatsheet](http://overapi.com/html-dom/)

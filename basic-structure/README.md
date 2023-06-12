# Basic Structure

### Doctype

All HTML documents must start with a &lt;!DOCTYPE&gt; declaration. \
The declaration is not an HTML tag. It is an "information" to the browser about what document type to expect. \
In HTML5, the &lt;!DOCTYPE&gt; declaration is simple:

```html
<!DOCTYPE html>
```

> Tip: The &lt;!DOCTYPE&gt; declaration is NOT case sensitive.

### html

The &lt;html&gt; tag represents the root of an HTML document. \
The &lt;html&gt; tag is the container for all other HTML elements (except for the &lt;!DOCTYPE&gt; tag).

```html
<!DOCTYPE html>
<html lang="en">
  ...Any other HTML tag
</html>
```

> Note: You should always include the lang attribute inside the &lt;html&gt; tag, to declare the language of the Web page. This is meant to assist search engines and browsers.

### head

The &lt;head&gt; element is a container for metadata (data about data) and is placed inside &lt;html&gt; and beside &lt;body&gt; \
Metadata is data about the HTML document. Metadata is not displayed. \
Metadata typically define the document title, character set, styles, scripts, and other meta information.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    ...Any other HTML metadata tag
  </head>
</html>
```

### body

The <body> tag defines the document's body. \
The <body> element contains all the contents of an HTML document, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.\

```html
<html>
  <body>
    ...Any other HTML content tag
  </body>
</html>
```

> Note: There can only be one <body> element in an HTML document.

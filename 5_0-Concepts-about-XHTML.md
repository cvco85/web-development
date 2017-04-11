# XHTML

XHTML (Extensible HyperText Markup Language) is a language that derived from XML (Extensible Markup Language) and HTML (HyperText Markup Language). Nowadays, the majority of websites are written in HTML even though the browsers still support XHTML.

XHTML or HTML are used to define a website structure.

Is is way more stricter than HTML, however, it is being less and less used, loosing ground to HTML.

## Syntax and rules

1. Elements must be well formed (must have starting and closing tags)

Example:

```html
<!--  Not valid -->
<div><i>Test</div></i>

<!-- Valid -->
<div><i>Test</i></div>
```

2. All elements and attribute names must be lowercase

As XML is case sensitive and XHTML derives from that, elements must be lowercase.

Example:

```html
<!-- Works -->
<div>Test div</div>

<!-- Doesn't work -->
<DIV>Test div</DIV>
```

3. Attribute values must be quoted

In XHTML, every attribute value must be quoted.

Example:

```html
<!-- Works -->
<div class="header">Test div</di>

<!-- Doesn't work -->
<div class=header>Test div</di>
```

4. Attribute minimization is not allowed

In HTML you can do things like `<textarea readonly >` where in XHTML you have to do `<textarea readonly="readonly">`.

5. Empty elements still need to be closed

Even when it's an empty element, it must be closed in order for XHTML to work.

```html
<!-- Works -->
<button />

<!-- Doesn't work -->
<button>
```

Nowadays, those strict XHTML are mostly used as best practices to write HTML, rather than directly to write XHTML.

______


## Structure

XHTML pages are composed by 4 elements:

- html (the root element where everything is inside)
- head (element that contains information about the current document)
- title (element that contains the page title)
- body (page main element, contains all the content)


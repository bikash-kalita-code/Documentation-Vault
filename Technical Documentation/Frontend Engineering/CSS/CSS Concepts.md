Like HTML, CSS is not a programming language. It's not a markup language either. **CSS is a style sheet language.** CSS is what you use to selectively style HTML elements.

#### Anatomy of a CSS ruleset
![[CSS Ruleset.png]]
#### Modify multiple property values in one ruleset
```css
p {
  color: red;
  width: 500px;
  border: 1px solid black;
}
```
#### Selecting Multiple Elements
```css
p,
li,
h1 {
  color: red;
}
```

### Different types of selectors
|Selector name|What does it select|Example|
|---|---|---|
|Element selector (sometimes called a tag or type selector)|All HTML elements of the specified type.|`p`  <br>selects `<p>`|
|ID selector|The element on the page with the specified ID. On a given HTML page, each id value should be unique.|`#my-id`  <br>selects `<p id="my-id">` or `<a id="my-id">`|
|Class selector|The element(s) on the page with the specified class. Multiple instances of the same class can appear on a page.|`.my-class`  <br>selects `<p class="my-class">` and `<a class="my-class">`|
|Attribute selector|The element(s) on the page with the specified attribute.|`img[src]`  <br>selects `<img src="myimage.png">` but not `<img>`|
|Pseudo-class selector|The specified element(s), but only when in the specified state. (For example, when a cursor hovers over a link.)|`a:hover`  <br>selects `<a>`, but only when the mouse pointer is hovering over the link.|

#### Fonts  and text
https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/CSS_basics#fonts_and_text

#### Comments
Anything in CSS between `/*` and `*/` is a **CSS comment**. The browser ignores comments as it renders the code.


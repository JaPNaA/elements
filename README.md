# elements

elements.js and elements.ts small utility library

## Usage

Download elements.js or elements.ts and insert it into your codebase.

Import the file as a JavaScript module.

```javascript
import { Elm, InputElm, Component } from "./elements.js";
```

### Elm

```javascript

let myElm;

new Elm().append(
  new Elm("h4").append("elements.js/ts"),
  new Elm().append("is a simple javascript element tree building utility library"),
  new Elm("br"),
  new Elm().class("container").append(
    myElm = new Elm().append("Elms can be stored in variables.")
  )
).appendTo(document.body);

myElm.replaceContents("and be changed later");

```

Above code generates HTML in DOM:

```html
<div>
  <h4>elements.js/ts</h4>
  <div>is a simple javascript element tree building utility library</div>
  <br>
  <div class="container">
    <div>and be changed later</div>
  </div>
</div>
```

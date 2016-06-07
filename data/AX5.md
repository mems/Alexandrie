# Form submition with button send button's text

When a form is submited with `<button type="submit" name="myButton" value="foo">Click me</button>`, the POST data send will result in `myButton=Click me` (equal `button.textContent`) instead of `myButton=foo`.

Tags:

-   form

Applications:

-   ✅ IE 7
-   ❎ IE 8

Links:

-   [\<button\> - HTML | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Button#Notes)
-   AX5


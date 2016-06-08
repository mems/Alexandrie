# Form data set contains submitter label instead of value

When a form is submitted from an submitter (`<button type="submit" name="bt" value="foo">Send</button>`), the data set will contains the button label (`bt=Send`) instead of its value (`bt=foo`).

Workaround: use `<input type="submit" value="foo">`, but you the button's label will be equal to the `value` attribute (`foo`).

## Tags

-   form

## Applications

-   ✅ IE 7
-   ❎ IE 8

## See also

-   [\\<button\> - HTML | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Button#Notes)
-   # AX7



# Port number is specified for anchor elements with unspecified port URL

For the document `http://domain.com/` with a link `<a href="http://domain.com/">link</a>` it give:

- `window.location.port == ""`
- `document.location.port == ""`
- `anchorElement.port == 80`

For the document `https://domain.com/` with a link `<a href="https://domain.com/">link</a>` it give:

- `window.location.port == ""`
- `document.location.port == ""`
- `anchorElement.port == 443`

Should be:

- `window.location.port == ""`
- `document.location.port == ""`
- `anchorElement.port == ""`

## Applications

-   ✅ IE11

## Tags

-   anchor
-   url
-   dom


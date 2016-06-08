# Port specified for anchor elements with unspecified port URL

The document `http://domain.com/` with a link `<a href="http://domain.com/">link</a>` give `window.location.port == "" && document.location.port == "" && anchorElement.port == 80`
The document `https://domain.com/` with a link `<a href="https://domain.com/">link</a>` give `window.location.port == "" && document.location.port == "" && anchorElement.port == 443`

Should be `anchorElement.port == ""`

## Applications

-   ✅ IE11

## Tags

-   anchor
-   url
-   dom


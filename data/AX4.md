# Leading slash missing for `anchorElement.pathname`

For `<a href="https://domain.com/path">link</a>` give `anchorElement.pathname == "path"`, should be `"/path"`.

Note: It's not the case for `document.location` and `window.location`.

Applications:

-   ✅ IE 9
-   ❎ IE1

Tags:

-   dom
-   url
-   anchor

Links:

-   [internet explorer - Javascript .pathname IE quirk? - Stack Overflow](http://stackoverflow.com/questions/956233/javascript-pathname-ie-quirk)
-   [\#3478 (Missing slash in location.pathname under Internet Explorer 10) – OpenLayers 2](http://trac.osgeo.org/openlayers/ticket/3478)
-   [HTMLHyperlinkElementUtils.pathname - Web APIs | MDN](https://developer.mozilla.org/en-US/docs/Web/API/URLUtils.pathname)
-   [February | 2011 | IEInternals](http://blogs.msdn.com/b/ieinternals/archive/2011/02/28/internet-explorer-window-location-pathname-missing-slash-and-host-has-port.aspx)


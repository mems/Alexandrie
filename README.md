# Alexandrie

Specificities of softwares that parse, render, deliver webpages and emails

Softwares include web server, web browsers, webmail, email clients, softwares with embedded web browser engine (like WebKit), proxies, etc.

Affected domains like CSS, HTML, JS, SVG, DOM, ARIA, WebGL, PNG, HTTP, etc. (see [W3C standards](http://www.w3.org/standards/)).

See also:

- [Outdated Browser](http://outdatedbrowser.com)
- [The myth of the “modern browser” | Christian Heilmann](http://christianheilmann.com/2012/08/03/the-myth-of-the-modern-browser/)

## Motivations

- we don't know everythink. We can miss things that create bugs
- there is not always a public bugtracking ticket for that. (Especially for proprietary softwares or old browsers like IE<11)
- we don't have a common test data available anywhere (lot of sources, when it's available)
- bug tracking don't often include metadatas (tests, links to more informations, details and explainations) and noisy informations (comments in same place, because it's a bugtracking!)
- bug tracking are for bugs, not for specifications interpretations nor for browser vendor specific features
- for the same bug, there is multiple tickets over multiple bugtracking (for each browser vendor) or too specific (internal implementations)
- we need discussions. Bug tracking ticket are not always allow that (Github Issues will let us do that)
- we want to know workaround, polyfills, etc.
- help us to dev with automations: 
	* generate definitions base on standards and softwares specifities (see Intellji: JavaScriptLanguage package with `@browser` annotation. See `com.intellij.lang.javascript.JavascriptLanguage`, ECMAScript.js, DHTML.js and HTML5.js)
	* generate documentation ([DevDocs](http://devdocs.io/))
	* update it (moz wiki, webplatform, caniuse)
	* create tools like: [The API Catalog](https://developer.microsoft.com/en-us/microsoft-edge/platform/catalog/)
	* linting (compability checking) for tools like:
		- https://github.com/anandthakker/doiuse
		- [I want to use](http://www.iwanttouse.com/)
		- ESLint (`--env`)
		- JSHint (http://jshint.com/docs/options/#browser)
		- JSLint (Assume browser, Node.js, etc.)
		- [israelidanny/ie8linter](https://github.com/israelidanny/ie8linter)
		- [JS Compatibility Checker](http://jscc.info/)
	* generate summaries [What CSS prefixes should I use?](http://shouldiprefix.com/)
- we want to know what the specs say and their implementation
	Embed a widget with support in blog etc. "browser support", similar to https://github.com/andismith/caniuse-widget or https://github.com/ireade/caniuse-embed/
- because old version of softwares are still used
- because when it's maintained, it done only by few people (projects other than caniuse, moz wiki, webplatform, etc.)
- because it's not the goal of our sources
- what specs say (if any)
- we have to live with it, but we should know to handle it
- when you remove old support or code/lib, you need to know exactly what can be removed

## Potential issues

- (data sources) [Circular reporting](https://en.wikipedia.org/wiki/Circular_reporting): can potentially resolved by tests (automatic and manually with aid)
- Data exactitude (contributor and test)
- (autotest) [undetectables](https://github.com/Modernizr/Modernizr/wiki/Undetectables) features (see also: [Form Inputs: The Browser Support Issue You Didn’t Know You Had – Smashing Magazine](http://www.smashingmagazine.com/2015/05/05/form-inputs-browser-support-issue/))
- large number of files in folder: https://git-annex.branchable.com/tips/Repositories_with_large_number_of_files/
- (contribution) require review (duplicate entries)

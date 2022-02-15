# Highlight.js GraphQL

> NOTE: GraphQL is now included in [highlight.js](https://github.com/highlightjs/highlight.js) and no longer maintained here.

Support for using `highlight.js` to syntax highlight GraphQL queries. See https://highlightjs.org/ for more information about highlight.js.

See https://graphql.org/ for more information about GraphQL. Query syntax is described in http://spec.graphql.org/June2018/.

**Built with**

* [highlightjs](https://github.com/highlightjs/highlight.js)

## Installation

Include the Highlight.js library in your webpage or Node app, then load this module.

### Static website

Load the GraphQL module after loading Highlight.js.  Use the minified version found in the `dist` directory.  This module is just a CDN build of the language, so it will register itself as the JavaScript is loaded.

```html
<script type="text/javascript" src="/path/to/highlight.min.js"></script>
<script type="text/javascript" src="/path/to/graphql.min.js"></script>
<script type="text/javascript">
  hljs.highlightAll();
</script>
```

### Using directly from the UNPKG CDN

```html
<script type="text/javascript"
  src="https://unpkg.com/highlightjs-graphql@0.1.0/dist/graphql.min.js"></script>
```

- More info: <https://unpkg.com>

### With Node or another build system

If you're using Node / Webpack / Rollup / Browserify, etc., require the language module, then register it with Highlight.js.

```javascript
var hljs = require('highlight.js');
var hljsGraphQL = require('highlightjs-graphql');

hljs.highlightAll();
```

## Usage

Once loaded, mark the code you want to highlight with the `language-graphql` class:

```html
<pre><code class="language-graphql">...</code></pre>
```

Without specifying the language, Highlight.js will attempt to auto-detect the grammar. Sometimes it is easier/better to tell highlight.js which language grammar to use instead of asking it to guess.

For more information, follow instructions at [highlightjs.org](https://highlightjs.org/usage/) to learn how to include the library and CSS and other use cases. See [Getting started](https://github.com/highlightjs/highlight.js#getting-started) for different integration and module options.

## License

Distributed under the [BSD 3-Clause](./LICENSE). See `LICENSE` for more information.

Highlight.js is released under the [BSD 3-Clause License](https://github.com/highlightjs/highlight.js/blob/master/LICENSE).

## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork this project.
2. Create a work branch (`git checkout -b my-branch`).
3. Commit your changes (`git commit -m 'my changes'`).
4. Push the branch (`git push origin my-branch`).
5. Open a Pull Request from your fork back to this repository.

## Links

- The official site for the Highlight.js library is <https://highlightjs.org/>.
- The Highlight.js GitHub project: <https://github.com/highlightjs/highlight.js>
- Learn more about GraphQL: <https://graphql.org>

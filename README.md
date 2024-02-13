# [WGSL](https://www.w3.org/TR/WGSL/) module for highlightjs

[![Apache 2.0](https://img.shields.io/badge/license-Apache-blue.svg)](#license)

## Usage

Simply include the Highlight.js library in your webpage or Node app, then load this module.
See the [highlight.js usage](https://github.com/highlightjs/highlight.js#basic-usage) page
for more details.

### Static website or simple usage

Load the module (found in the `dist` directory):

```html
<script type="text/javascript" src="/path/to/highlight.min.js"></script>
<script type="text/javascript" src="/path/to/highlightjs-wgsl/dist/wgsl.min.js"></script>
<script type="text/javascript">
	hljs.highlightAll();
</script>
```

### With Node or another build system

If you're using Node / Webpack / Rollup / Browserify, etc, simply require the language
module, then register it with Highlight.js.

```javascript
var hljs = require('highlightjs');
var hljsWgsl = require('highlightjs-wgsl');

hljs.registerLanguage("cypher", hljsWgsl);
hljs.highlightAll();
```

## License

See the [LICENSE](/LICENSE.md) file.

## Contribution

Contributions are welcome by pull request.

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall be
licensed as above, without any additional terms or conditions.

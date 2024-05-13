# @gorner/broccoli-templater

broccoli plugin that combines lodash's `_.template` and broccoli for fun stuff.

Fork of Stefan Penner's [broccoli-templater](https://github.com/stefanpenner/broccoli-templater)
but with unmaintained `lodash.template` replaced with regular lodash due to vulnerabilities.

## example:

```js
var templatedTree = new Template(untemplatedTree, pathToTemplate,
  function buildVariables(content, relativePath) {
    return {
      moduleBody: content
    };
});
```

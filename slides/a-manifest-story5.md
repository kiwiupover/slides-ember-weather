##  A Manifest Story

#### ember-cli-build.js
```js
module.exports = function(defaults) {
  var options = {
    storeConfigInMeta: false,
    vendorFiles: {
     'jquery.js': false,
     'handlebars': false
    }
  };

  var app = new EmberApp(defaults, options);
};
```

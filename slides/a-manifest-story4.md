##  A Manifest Story

#### app/initializers/config.js
```js
var WindowConfig = function(){
  return window.config;
};

var configFactory = new WindowConfig();

export function initialize(container, application) {
  application.register('config:main',  configFactory, { instantiate: false });
  application.inject('component', 'config', 'config:main');
  application.inject('route', 'config', 'config:main');
  application.inject('model', 'config', 'config:main');
  application.inject('controller', 'config', 'config:main');
}

export default {
  name: 'gdconfig',
  initialize: initialize
};

```

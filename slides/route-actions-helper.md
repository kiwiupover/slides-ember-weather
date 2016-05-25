##  Route Actions Helper

### passing clousure actions
<span class="white">
http://emberobserver.com/addons/ember-route-action-helper
</span>

<br><br>
```hbs
{{my-component submit=(route-action 'saveTheModel')}}
```

```js
import Ember from 'ember';

export default Ember.Component.extend({
  actions: {
    submit(){
      this.attrs.submit();
    }
  }
});
```

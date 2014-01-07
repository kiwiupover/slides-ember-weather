##  Ember Data

#### Find a record
```javascript
  Pos.OrderRoute = Ember.Route.extend({
    model: function(params) {
      return this.store.find('order', params.order_id);
    }
  });
```
####Create & Persist a record
```javascript
  var lineItem = {
    name: this.get('name'),
    priceCents: this.get('priceCents'),
    taxable: this.get('taxable')
  };

  lineItem = this.store.createRecord('lineItem', lineItem);

  lineItem.save();
```


<div class="number"><sup>#</sup>5</div>

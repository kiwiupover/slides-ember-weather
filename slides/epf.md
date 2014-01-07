##  Ember Persistent Foundation

### Flushes your model graph

```javascript
  var lineItem = {
    name: this.get('name'),
    priceCents: this.get('priceCents'),
    taxable: this.get('taxable')
  };
  lineItem = this.session.create('lineItem', lineItem);
  session.flush();
```

<div class="number"><sup>#</sup>5</div>

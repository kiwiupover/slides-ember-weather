##  Routing is Easy

####Routing a JS frontend is no longer naff!

```Javascript
Pos.Router.map(function() {
  this.resource('orders', function() {
    this.resource('order', {path:':order_id'}, function() {
      this.route('payment');
      this.route('edit');
    });
    this.route('new');
  });
  this.resource('products', function(){
    this.route('show', {path: ':product_id'});
    this.route('edit', {path: ':product_id/edit'});
  });
});
```
<div class="number"><sup>#</sup>3</div>

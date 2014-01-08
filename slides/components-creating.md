##Creating Components

```javascript
Pos.ProductPanelComponent = Em.Component.extend({
  tagName: 'li',
  classNameBindings: ["category.categorySlug"],

  click: function() {
    this.sendAction('action', this.get('product'));
  }
});
```

```hanblebars
<a href="">
  <div class='panel'>
    <h4>{{product.name}}</h4>
    <p class='mbn'>
      {{product.shortDescription}}
    </p>
    <div class="money">
      ${{money product.priceCents}}
    </div>
  </div>
</a>
```
<div class="number"><sup>#</sup>10</div>

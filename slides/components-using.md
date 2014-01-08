##Using a Component


```hanblebars
<h3>{{name}}</h3>
<ul class="products-list">
  {{#each product in products}}
    {{product-panel product=product
                    category=model
                    action="addListItem"}}
  {{/each}}
</ul>
```
<div class="number"><sup>#</sup>10</div>

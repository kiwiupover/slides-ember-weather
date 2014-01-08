##Active Model Serializers

```Ruby
class ProductSerializer < ActiveModel::Serializer
  attributes :id, :name, :description, :price_cents, :category

  attribute :short_description

  def short_description
    (description[0..40] + "...") if description
  end

end
```

<div class="number"><sup>#</sup>9</div>

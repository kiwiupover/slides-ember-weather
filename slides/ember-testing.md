##  Ember Testing

```coffeescript
test "as an owner, I should see my restaurants in Owner Dash", ->
  visit("/").then ->
    equal find("h3").first().text(), "Login", "Expect to see login message"
    fillIn "#login_username input", "owner@urbanspoon.com"
    fillIn "#login_password input", "pppppp"
    click("#login-button").then ->
      equal find("h2").first().text(), "Lord of the Fries", "Expect to see the Restaurant title"
```

<div class="number"><sup>#</sup>13</div>

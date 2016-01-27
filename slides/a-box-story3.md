##  A Box Story

```ruby
require "ember-cli/deploy"

class ApplicationController < ActionController::Base
  def index
    @deploy = EmberCLI::Deploy::Redis.new(namespace: "frontend")

    user = render_to_string(partial: "user", current_user)

    @deploy.append_to_body(user)

    render text: @deploy.html, layout: false
  end
  # ...
end
```

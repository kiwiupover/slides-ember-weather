## lightning in Rails

```ruby
require "ember-cli/deploy"

class ApplicationController < ActionController::Base
  def index
    @deploy = EmberCLI::Deploy::Redis.new(namespace: "frontend")

    head = render_to_string(partial: "my_csrf_and_metadata")
    body = render_to_string(partial: "my_analytics")

    @deploy.append_to_head(head)
    @deploy.append_to_body(body)

    render text: @deploy.html, layout: false
  end
  # ...
end
```

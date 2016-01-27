## lightning in Rails

```ruby
require "ember-cli/deploy/redis"

class ApplicationController < ActionController::Base
  def index
    @deploy = EmberCLI::Deploy::Redis.new(namespace: "frontend")

    render text: @deploy.html, layout: false
  end
end
```
[EmberCLI::Rails - Deploy Redis](https://github.com/seanpdoyle/ember-cli-rails-deploy-redis)

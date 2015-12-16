# PBX-Client

Dynamically generates a JavaScript client based on PBX API description.

```coffee
client = require "pbx-client"

client.discover "http://api.acme.com"
.then (api) ->
  api.widgets.get()
  .then (response, body) ->
    body.then (widgets) ->
      # do something with widgets...
```

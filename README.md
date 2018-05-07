### Nanoleaf

From Section 7 of the [Nanoleaf Open API Reference](http://forum.nanoleaf.me/docs/openapi). Requires setting up a developer account and signing in to their developer portal.

Click the Run in Postman button below to import this Postman Collection and Environment into your local instance of the [Postman app](https://www.getpostman.com/apps).

[insert RIP button]

### Generate an authorization token by:

1. Holding the on-off button for 5-7 seconds on the Nanoleaf controller until the LED starts flashing in a pattern.
2. Sending a POST request to the authorization endpoint within 30 seconds of activating pairing, like this (substituting the IP address and port for your central controller):

`http://192.188.x.x:16021/api/v1/new`

The result returned will be a 32-character authorization token that you will use in all of your subsequent calls.

### Quickstart:

I added a Quickstart folder to demonstrate a possible workflow (visible in the pre-request and test script sections). The remaining folders are replicated from the [Nanoleaf Open API Reference](http://forum.nanoleaf.me/docs/openapi). For more details and to see example responses, check out the [collection documentation](insert link here).

[Update the Postman environment](https://www.getpostman.com/docs/v6/postman/environments_and_globals/manage_environments#editing-an-active-environment) with your IP and port.

If you already have an authorization token, update the Postman environment with your token. Otherwise, you will need to use the [Add a user](insert collection docs link) to generate an authorization token.


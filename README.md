### Nanoleaf

From Section 7 of the [Nanoleaf Open API Reference](http://forum.nanoleaf.me/docs/openapi). Requires setting up a developer account and signing in to their developer portal.

![[nanoleaf logo](https://s3.amazonaws.com/postman-static-getpostman-com/postman-docs/nanoleaf-logo.png)](https://s3.amazonaws.com/postman-static-getpostman-com/postman-docs/nanoleaf-logo.png)

Click the Run in Postman button below to import this Postman Collection and Environment into your local instance of the [Postman app](https://www.getpostman.com/apps).

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/b6c8948a002d2dcd6364#?env%5BNanoleaf%5D=W3sia2V5IjoiaXBBZGRyZXNzIiwidmFsdWUiOiIxOTIuMTY4LngueDoxNjAyMSIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJ0ZXh0In0seyJrZXkiOiJhdXRoVG9rZW4iLCJ2YWx1ZSI6IkFkZC1hLXVzZXItdG8tZ2VuZXJhdGUtYXV0aC10b2tlbiIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJ0ZXh0In1d)

### Generate an authorization token

1. On the Nanoleaf controller, hold the on-off button for 5-7 seconds until the LED starts flashing in a pattern.
2. From the Postman app or your own app, send a POST request to the authorization endpoint within 30 seconds of activating pairing, like this (substituting the IP address and port for your central controller):

`http://192.188.x.x:16021/api/v1/new`

The result returned will be a 32-character authorization token that you will use in all of your subsequent calls.

### Quickstart

[Update the Postman environment](https://www.getpostman.com/docs/v6/postman/environments_and_globals/manage_environments#editing-an-active-environment) with your IP and port.

1. If you already have an authorization token, update the Postman environment with your token. Otherwise, you will need to use the [Add a user](insert collection docs link) `POST` request to generate an authorization token.
2. In this Postman collection, I added a Quickstart folder to group a handful of requests to demonstrate a possible workflow (visible in the pre-request and test script sections). The remaining folders are replicated from the [Nanoleaf Open API Reference](http://forum.nanoleaf.me/docs/openapi). For more details and to see example responses, check out the [collection documentation](insert link here).

[insert screenshot of documentation]

# Front End Client APIs

Client APIs support the implementation of the Simple Store API into public facing channels like a web or mobile application.

### API Key

All Front End Client APIs must include an API Key which is associated with your Simple Store \(Tenant\) Account.

the API key is passed onto each request using the header: x-api-key

### Token Authentication

A subset of the Client API support functionality tied to specific customers, examples include:

* Change Customer Details
* Change Password
* Get Order History

A token is issued by calling the [\[login\]](https://clients.api.simplestore.io/swagger/index.html#/Customer/Customer_Login) method on the Client API:

```bash
curl -d '{"emailAddress":"email address", "password":"password"}' \
     -H "Content-Type: application/json" \
     -H "x-api-key: [api-key]"
     -X POST https://clients.api.simplestore.io/v1/customer/login
```




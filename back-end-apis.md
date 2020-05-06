# Backend APIs

The Simple Store Backend API support system to system integration to allow the building of complete applications using the Simple Store Platform.  Example integrations include:

* Server Side Framework \(Spring/MVC\) to Simple Store
* Backend System \(Order Management, Product Supplier\) to Simple Store

### Client Credential Authentication

SimpleStore platform uses bearer token to authenticate API requests. Using OAuth client credentials to authenticate the calling application and return a token that is valid for 60 minutes.

This token then used as a Bearer Token for subsequent API calls to the platform.

{% hint style="warning" %}
`client_secret`is sensitive information and it should never used or disclosed publicly.
{% endhint %}

## Get an Access Token

This endpoint responsible in generating access tokens for Client \(application\) to allow full read and write access to the platform.

### **POST**

```text
https://auth.simplestore.io/connect/token
```

#### Request: Headers

| Key | Value |
| :--- | :--- |
| Content-Type | application/x-www-form-urlencoded |

#### Request: Route

No Route

#### Request: Query

No Query

#### Request: Body

{% tabs %}
{% tab title="Request Object" %}
| Element | Type | Description |
| :--- | :--- | :--- |
| grant\_type | string | "client\_credentials" |
| client\_id | string | Your client\_id generated from Control Panel |
| client\_secret | string | Your client\_secret generated from Control Panel |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "grant_type" : "client_credentials"
  "client_id" : [from control panel]
  "client_secret" : [from control panel]
}
```
{% endtab %}
{% endtabs %}

#### Response: 200 Ok

Successful authentication of client credentials will return access token with expiry time in seconds.

{% hint style="info" %}
`access_token`has an expiry of 60 minutes. You must renew the token on or before expiry.
{% endhint %}

{% tabs %}
{% tab title="Response Object" %}
| Element | Type | Description |
| :--- | :--- | :--- |
| access\_token | string | A token |
| expiries\_in | int | 3600 |
| token\_type | string | "Bearer" |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
    "access_token": "<Token>",
    "expires_in": 3600,
    "token_type": "Bearer"
}
```
{% endtab %}
{% endtabs %}

#### Response: 400 Bad Request

Failed authentication will return invalid client

{% tabs %}
{% tab title="Response Object" %}
| Element | Type | Desciption |
| :--- | :--- | :--- |
| error | string | error description |
| title | string |  |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
    "error": "invalid_client"
}
```
{% endtab %}
{% endtabs %}


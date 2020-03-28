# Authentication

SimpleStore platform uses bearer token to authenticate API requests. Using OAuth client credentials to authenticate the calling application and return a token that is valid for 60 minutes.

This token then used as a Bearer Token for subsequent API calls to the platform.

{% hint style="warning" %}
`client_secret`is sensitive information and it should never used or disclosed publicly.
{% endhint %}

{% api-method method="post" host="https://auth.simplestore.io" path="/connect/token" %}
{% api-method-summary %}
Access Token
{% endapi-method-summary %}

{% api-method-description %}
This endpoint responsible in generating access tokens for Client \(application\) to allow full read and write access to the platform.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Content-Type" type="string" required=true %}
application/x-www-form-urlencoded
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-form-data-parameters %}
{% api-method-parameter name="grant\_type" type="string" required=true %}
`client_credentials`
{% endapi-method-parameter %}

{% api-method-parameter name="client\_id" type="string" required=true %}
Your `client_id` generated from Control Panel
{% endapi-method-parameter %}

{% api-method-parameter name="client\_secret" type="string" required=true %}
Your `client_secret` generated from Control Panel 
{% endapi-method-parameter %}
{% endapi-method-form-data-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful authentication of client credentials will return access token with expiry time in seconds
{% endapi-method-response-example-description %}

```javascript
{
    "access_token": "<Token>",
    "expires_in": 3600,
    "token_type": "Bearer"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=400 %}
{% api-method-response-example-description %}
Failed authentication will return invalid client
{% endapi-method-response-example-description %}

```
{
    "error": "invalid_client"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% hint style="info" %}
`access_token` has an expiry of 60 minutes. You must renew the token on or before expiry.
{% endhint %}


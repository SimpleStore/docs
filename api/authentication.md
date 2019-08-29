# Authentication

SimpleStore API uses bearer token to authenticate requests. To generate a Token, client credentials are use to call the Auth service to retrieve a token.

{% api-method method="post" host="https://auth.simplestore.io" path="/connect/token" %}
{% api-method-summary %}
Get Cakes
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get free cakes.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Content-Type" type="string" required=true %}
application/x-www-form-urlencoded
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-body-parameters %}
{% api-method-parameter name="grant\_type" type="string" required=true %}
client\_credentials
{% endapi-method-parameter %}

{% api-method-parameter name="client\_id" type="string" required=true %}
Client id
{% endapi-method-parameter %}

{% api-method-parameter name="client\_secret" type="string" required=true %}
Client secret
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
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




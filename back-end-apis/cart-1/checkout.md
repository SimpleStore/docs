# Checkout

{% api-method method="post" host="https://api.simplestore.io" path="/v1/cart/{CartId}" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="cartId" type="string" required=true %}
A unique identifier for the cart
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="d" type="string" required=false %}

{% endapi-method-parameter %}

{% api-method-parameter name="s" type="string" required=true %}
d
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

Completes the check out process against the cart creating an order.

After checkout the Cart becomes a Basket.

### **POST**

```text
/v1/cart/{CartId}
```

#### Request: Route

| Element | Type | Description |
| :--- | :--- | :--- |
| cartId | guid/uuid | A unique identifier for the cart |

#### Request: Query

No Query

#### Request:  Body

{% tabs %}
{% tab title="Request Object" %}
| Element | Type | Description |
| :--- | :--- | :--- |
| customerId | guid | Unique Identifer for Customer |
| customerEmail | string | Customer Email Address |
| customerFirstName | string | Customer First Name |
| customerLastName | string | Customer Last Name |
| purchaserName | string | Purchaser \(Billing\) Name |
| purchaserContactNumberLocal | string | Purchase  \(Billing\) Contact Number |
| purchaserEmail | string | Purchase  \(Billing\) Email |
| recieverName | string | Receiver \(Shipping\) Name |
| receiverContactNumberLocal | string | Receiver \(Shipping\) Contact Number |
| receiverEmail | string | Receiver \(Shipping\) Email |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "customerId": "string",
  "customerEmail": "string",
  "customerFirstName": "string",
  "customerLastName": "string",
  "purchaserName": "string",
  "purchaserContactNumberLocal": "string",
  "purchaserEmail": "string",
  "receiverName": "string",
  "receiverContactNumberLocal": "string",
  "receiverEmail": "string"
}
```
{% endtab %}
{% endtabs %}

#### Response: 200 Success

{% tabs %}
{% tab title="Response Object" %}
| Element | Desciption |
| :--- | :--- |
| orderId | Unique Identifier for the Order |
| customerId | Unique Identifier for the Customer |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "orderId": "string",
  "customerId": "string"
}

```
{% endtab %}
{% endtabs %}

#### Response: 404 Not Found

{% tabs %}
{% tab title="Response Object" %}
| Element | Type | Desciption |
| :--- | :--- | :--- |
| type | string |  |
| title | string |  |
| status | int |  |
| detail | string |  |
| instance | string |  |
| extensions | object |  |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "type": "string",
  "title": "string",
  "status": 0,
  "detail": "string",
  "instance": "string",
  "extensions": {}
}
```
{% endtab %}
{% endtabs %}

#### 




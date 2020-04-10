# Calculate Shipping

Applies a Country and State to a Cart and calculates Shipping.

### **POST**

```text
/v1/cart/{CartId}/shipping
```

#### Request: Route

| Element | Type | Description |
| :--- | :--- | :--- |
| cartId | guid/uuid | A unique identifier for the cart |

#### Request:  Body

{% tabs %}
{% tab title="Request Object" %}
| Element | Type | Description |
| :--- | :--- | :--- |
| country | string | ISO Country Code |
| state | string | State / Province / Region |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "country": "string",
  "state": "string"
}
```
{% endtab %}
{% endtabs %}

#### Response: 200 Success

Cart Object \(See [Cart](./)\)

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


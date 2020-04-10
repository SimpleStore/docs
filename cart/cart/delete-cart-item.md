# Delete Cart Item

Deletes an Item from the Cart.

### **DELETE**

```text
/v1/cart/{CartId}/items
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
| items | array | Cart Item Array |
| items\[\].productId | string | ProductId \(See [Product](../../catalog-1/product.md)\) |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "items": [
    "string"
  ]
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


# Create/Update Cart Item

Adds or updates a Product as an Item to the Cart.

The Cart Item is updated if the ProductId already exists in the Cart.  
  
Creates a Cart for a new cartId if a new CartId is provided.

If no CartId is provided a new Cart and CartId is created and the CartId is returned.

Carts are transient and expire after 14 days.

### **POST**

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
| currencyCode | string | ISO Currency Code |
| items | array | Cart Item Array |
| items\[\].productId | string | ProductId \(See [Product](../../catalog/product.md)\) |
| items\[\].quantity | int | Quantity of Product |
| attributes | object | Attributes are a list of Key/Value to support customisation of the cart items |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "currencyCode": "string",
  "items": [
    {
      "productId": "string",
      "quantity": 0
    }
  ],
  "attributes": {}
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


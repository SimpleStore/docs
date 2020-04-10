# Get Cart By Cart Id

###  **GET**

```text
/v1/cart/{CartId}
```

#### Request: Route

| Element | Type | Description |
| :--- | :--- | :--- |
| cartId | guid/uuid | A unique identifier for the cart |

#### Request: Body

No request body

#### Response: 200

Success

{% tabs %}
{% tab title="Attributes" %}
| Element | Desciption |
| :--- | :--- |
| cartId | Unique Identifier for the Cart |
| items\[\] | An array of one or many items in the Cart |
| item.productId | Unique Identifer for the Product \(see [Product](../../catalog-1/product.md)\) |
| item.slug | Product Slug |
| item.title | Product Title |
| item.description | Product Description |
| item.quanity | Quantity of Product |
| item.paymentMethod | Payment Method |
| item.totalCurrency | Product Total in Currency |
| item.totalPoints | Product Total in Points |
| item.files\[\] | See [Assets](../../assets-1/assets.md) |
| item.attributes | One or more key/value pairs to support customisation of products |
| currencyCode | ISO currency code |
| shippingFee | Shipping Fee |
| subTotalCurrency | Cart Total in Currency \(excluding Shipping\) |
| totalCurrency | Cart Total in Currency |
| totalPoints | Cart Total in Points |
| attributes | One or more key/value pairs to support customisation of cart |
|  |  |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "cartId": "string",
  "items": [
    {
      "productId": "string",
      "slug": "string",
      "title": "string",
      "description": "string",
      "quantity": 0,
      "paymentMethod": "CurrencyOnly",
      "totalCurrency": 0,
      "totalPoints": 0,
      "files": [
        {
          "fileId": "string",
          "contentType": "string",
          "accessPermission": "string",
          "accessUrl": "string",
          "attributes": {},
          "edgeUrl": "string"
        }
      ],
      "attributes": {}
    }
  ],
  "currencyCode": "string",
  "shippingFee": 0,
  "subTotalCurrency": 0,
  "totalCurrency": 0,
  "totalPoints": 0,
  "attributes": {}

```
{% endtab %}
{% endtabs %}




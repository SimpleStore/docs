# Cart

Simple Store supports a full ecommerce shopping cart object.

### Basic Cart Process

![](../../.gitbook/assets/image%20%2814%29.png)

{% tabs %}
{% tab title="Attributes" %}
| Element | Desciption |
| :--- | :--- |
| cartId | Unique Identifier for the Cart |
| items\[\] | An array of one or many items in the Cart |
| items\[\].productId | Unique Identifer for the Product \(see [Product](../product.md)\) |
| items\[\].slug | Product Slug |
| items\[\].title | Product Title |
| items\[\].description | Product Description |
| items\[\].quanity | Quantity of Product |
| items\[\].paymentMethod | Payment Method |
| items\[\].totalCurrency | Product Total in Currency |
| items\[\].totalPoints | Product Total in Points |
| items\[\].files\[\] | See [Assets](../assets/) |
| items\[\].attributes | One or more key/value pairs to support customisation of products |
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
}
```
{% endtab %}
{% endtabs %}






# Cart

Simple Store supports a full ecommerce shopping cart.

{% tabs %}
{% tab title="Attributes" %}
| Element | Desciption |
| :--- | :--- |
| cartId | Unique Identifier for the Cart |
| items\[\] | An array of one or many items in the Cart |
| item.productId | Unique Identifer for the Product \(see [Product](../catalog-1/product.md)\) |
| item.slug |  |
| item.title |  |
| item.description |  |
| item.quanity |  |
| item.paymentMethod |  |
| item.totalCurrency |  |
| item.totalPoints |  |
| item.files\[\] | See [Assets](../assets-1/assets.md) |
| item.attributes |  |
| currencyCode |  |
| shippingFee |  |
| subTotalCurrency |  |
| totalCurrency |  |
| totalPoints |  |
| attributes |  |
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






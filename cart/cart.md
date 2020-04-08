# Cart

Simple Store supports a full ecommerce shopping cart.

{% tabs %}
{% tab title="Attributes" %}
| Element | Desciption |
| :--- | :--- |
| CartId | Unique Identifier for the Cart |
| Items\[\] | An array of one or many items in the Cart |
| Item.ProductId |  |



  
  


```text
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






# Get Basket By Cart Id

Searche for a Baskets \(a Cart that has completed checkout\) by Cart Id

### **GET**

```text
/v1/basket/bycart/{CartId}
```

#### Request: Route

| Element | Type | Description |
| :--- | :--- | :--- |
| CartId | guid | Unique Identifier for the Cart |

#### Request: Query

No Query

#### Request:  Body

No Request Body

#### Response: 200 Success

{% tabs %}
{% tab title="Response  Object" %}


| Element |  | Desciption |
| :--- | :--- | :--- |
| basketId | guid | Unique Identifier for the Cart |
| version | int | incremental version number of basket object |
| customerId | guid | Customer customerId |
| orderId | guid | Order orderId |
| status | string | status of Order |
| items\[\] | array | An array of one or many items in the Cart |
| items\[\].productId | guid | Unique Identifer for the Product \(see [Product](../../catalog-1/product.md)\) |
| items\[\].slug | string | Product Slug |
| items\[\].title | string | Product Title |
| items\[\].description | string | Product Description |
| items\[\].quanity | int | Quantity of Product |
| items\[\].paymentMethod | string | Payment Method |
| .items\[\].totalCurrency | decimal | Product Total in Currency |
| items\[\].totalPoints | decimal | Product Total in Points |
| items\[\].files\[\] | array | See [Assets](../../assets-1/assets.md) |
| items\[\].attributes | object | One or more key/value pairs to support customisation of products |
| items\[\]currencyCode | string | ISO currency code |
| shippingFee | decimal | Shipping Fee |
| subTotalCurrency | decimal | Cart Total in Currency \(excluding Shipping\) |
| totalCurrency | decimal | Cart Total in Currency |
| totalPoints | decimal | Cart Total in Points |
| attributes | object | One or more key/value pairs to support customisation of cart |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "result": [
    {
      "basketId": "string",
      "version": "string",
      "customerId": "string",
      "orderId": "string",
      "status": "Draft",
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
  ],
  "pageSize": 0,
  "pageIndex": 0,
  "totalRecordsFound": 0,
  "resultCount": 0,
  "totalPages": 0,
  "queryDurationMilliseconds": 0
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


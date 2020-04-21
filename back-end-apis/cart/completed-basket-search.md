# Basket Search

Searches for Baskets \(Carts that have completed checkout\)

### **GET**

```text
/v1/basket
```

#### Request: Route

No Route Values

#### Request: Query

| Element | Type | Description |
| :--- | :--- | :--- |
| CartId | array | An array of cartId\(s\) |
| IncludeItems | boolean | Include items in response |
| IncludeAttributes | boolean | Include attributes in response |
| PageSize | integer | Page Size.  The number of records returned. |
| PageIndex | integer | Page Index.  The page of records returned. |

#### Request:  Body

No Request Body

#### Response: 200 Success

{% tabs %}
{% tab title="Response  Object" %}


| Element |  | Description |
| :--- | :--- | :--- |
| result | array | array of carts |
| result\[\].basketId | guid | Unique Identifier for the Cart |
| result\[\].version | int | incremental version number of basket object |
| result\[\].customerId | guid | Customer customerId |
| result\[\].orderId | guid | Order orderId |
| result\[\].status | string | status of Order |
| result\[\].items\[\] | array | An array of one or many items in the Cart |
| result\[\].items\[\].productId | guid | Unique Identifer for the Product \(see [Product](../product.md)\) |
| result\[\].items\[\].slug | string | Product Slug |
| result\[\].items\[\].title | string | Product Title |
| result\[\].items\[\].description | string | Product Description |
| result\[\].items\[\].quanity | int | Quantity of Product |
| result\[\].items\[\].paymentMethod | string | Payment Method |
| result\[\].items\[\].totalCurrency | decimal | Product Total in Currency |
| result\[\].items\[\].totalPoints | decimal | Product Total in Points |
| result\[\].items\[\].files\[\] | array | See [Assets](../assets/) |
| result\[\].items\[\].attributes | object | One or more key/value pairs to support customisation of products |
| result\[\].items\[\]currencyCode | string | ISO currency code |
| result\[\].shippingFee | decimal | Shipping Fee |
| result\[\].subTotalCurrency | decimal | Cart Total in Currency \(excluding Shipping\) |
| result\[\].totalCurrency | decimal | Cart Total in Currency |
| result\[\].totalPoints | decimal | Cart Total in Points |
| result\[\].attributes | object | One or more key/value pairs to support customisation of cart |
| pageSize | int | Page Size |
| pageIndex | int | Page Index |
| totalRecordsFound | int | Total Records Found |
| resultCount | int | Result Count |
| totalPages | int | Total Pages |
| queryDurationMilliseconds | int | Query Duration in Milliseconds |
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
| Element | Type | Description |
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


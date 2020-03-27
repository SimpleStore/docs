# Product

A Product represents a product that can be purchased within the the Simple Store Platform.

The Product object comprises a both a standard set of default fields along with a flexible model to extend the product to meet your customisation needs.



  


```text
{
  "productId": "string",
  "slug": "string",
  "shortUrl": "string",
  "version": "string",
  "title": "string",
  "description": "string",
  "titles": {
    "additionalProp1": "string",
    "additionalProp2": "string",
    "additionalProp3": "string"
  },
  "descriptions": {
    "additionalProp1": "string",
    "additionalProp2": "string",
    "additionalProp3": "string"
  },
  "isActive": true,
  "status": "Available",
  "attributes": {},
  "categories": [
    {
      "key": "string",
      "value": "string",
      "slug": "string"
    }
  ],
  "collections": [
    {
      "key": "string",
      "value": "string",
      "slug": "string"
    }
  ],
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
  "paymentMethod": "RewardsOrCurrency"
}
```


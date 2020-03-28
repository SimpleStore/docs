# Product

A Product represents a product that can be purchased within the the Simple Store Platform.

The Product object comprises a both a standard set of default fields along with a flexible model to extend the product to meet your customisation needs.

<table>
  <thead>
    <tr>
      <th style="text-align:left">Element</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Slug</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Short Url</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Version</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Title</td>
      <td style="text-align:left">Default Title for Product</td>
    </tr>
    <tr>
      <td style="text-align:left">Description</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Titles</td>
      <td style="text-align:left">Dictionary for</td>
    </tr>
    <tr>
      <td style="text-align:left">Descriptions</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">IsActive</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Status</td>
      <td style="text-align:left">
        <p>Available</p>
        <p>OutOfStock</p>
        <p>Discontinued</p>
        <p>Unavailable</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Attributes</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Categories</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Collections</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Files</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Payment Method</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">BasePrice</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Price</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">BaseRewards</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Rewards</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Inventory</td>
      <td style="text-align:left"></td>
    </tr>
  </tbody>
</table>

  


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


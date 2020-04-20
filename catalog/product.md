# Product

A Product represents something that can be purchased within the the Simple Store platform.

The Product object comprises both a standard set of default fields along with a flexible model to extend the product to meet your customisation needs.

The Product can be associated with Categories, Collection, Assets and Attributes.

### Portal View

![](../.gitbook/assets/image%20%2827%29.png)

### Product Properties

{% tabs %}
{% tab title="Attributes" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left">Element</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">productId</td>
      <td style="text-align:left">Unique Identifer for the Product</td>
    </tr>
    <tr>
      <td style="text-align:left">slug</td>
      <td style="text-align:left">A Url slug used to identify a product</td>
    </tr>
    <tr>
      <td style="text-align:left">shortUrl</td>
      <td style="text-align:left">A globally unique id identifier (see <a href="../getting-started/quickbuy.md">QuickBuy</a>)</td>
    </tr>
    <tr>
      <td style="text-align:left">version</td>
      <td style="text-align:left">An incremental version number tracking changes to the Product configuration</td>
    </tr>
    <tr>
      <td style="text-align:left">title</td>
      <td style="text-align:left">Default Title for the Product</td>
    </tr>
    <tr>
      <td style="text-align:left">description</td>
      <td style="text-align:left">Default Description for the Product</td>
    </tr>
    <tr>
      <td style="text-align:left">titles</td>
      <td style="text-align:left">
        <p>Dictionary (key, value) of alternate Titles other languages to support
          internationalisation (i18n) and localisation (l10n):</p>
        <ul>
          <li>Key = ja-JP</li>
          <li>Value = &lt;Title in Japanese&gt;</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">descriptions</td>
      <td style="text-align:left">
        <p>Dictionary (key, value) of alternate Descriptions other languages to support
          internationalisation (i18n) and localisation (l10n), for example:</p>
        <ul>
          <li>Key = ja-JP</li>
          <li>Value = &lt;Description in Japanese&gt;</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">isActive</td>
      <td style="text-align:left">Active (True) or InActive (False)</td>
    </tr>
    <tr>
      <td style="text-align:left">status</td>
      <td style="text-align:left">
        <p>Available = Product is Available</p>
        <p>Out Of Stock = Product is Out of Stock</p>
        <p>Discontinued = Product has been discontinued</p>
        <p>Unavailable = Product is unavailable</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">attributes</td>
      <td style="text-align:left">Attributes are a list of Key/Value to support customisation of a product</td>
    </tr>
    <tr>
      <td style="text-align:left">categories</td>
      <td style="text-align:left">One or many categories the Product is assigned to (see <a href="categories.md">Categories</a>)</td>
    </tr>
    <tr>
      <td style="text-align:left">collections</td>
      <td style="text-align:left">One or many collections the Product is assigned to (see <a href="collections.md">Collections</a>)</td>
    </tr>
    <tr>
      <td style="text-align:left">files[]</td>
      <td style="text-align:left">One or many assets associated with the Product (see <a href="../back-end-apis/assets.md">Assets</a>)</td>
    </tr>
    <tr>
      <td style="text-align:left">paymentMethod</td>
      <td style="text-align:left">
        <p>Defines the supported payment methods for a product:</p>
        <p>CurrencyOnly = Can be paid with by currency ONLY, not eligible to be paid
          for with points</p>
        <p>RewardsOrCurrency = Can be paid with currency or rewards points in full</p>
        <p>RewardsOnly = Can be paid in rewards points ONLY</p>
        <p>RewardsPlusPay = Can be paid with a mix of currency and points</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">basePrice</td>
      <td style="text-align:left">See <a href="pricing.md">Pricing</a>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">price</td>
      <td style="text-align:left">See <a href="pricing.md">Pricing</a>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">baseRewards</td>
      <td style="text-align:left">See <a href="rewards.md">Rewards </a>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">rewards</td>
      <td style="text-align:left">See <a href="rewards.md">Rewards </a>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">inventory</td>
      <td style="text-align:left">See <a href="inventory.md">Inventory</a>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="Sample Object" %}
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
  "paymentMethod": "CurrencyOnly",
  "basePrice"	{}
  "price"	{}
  "baseRewards"	{}
  "rewards"	{}
  "inventory"	{}
}
```
{% endtab %}
{% endtabs %}

#### 


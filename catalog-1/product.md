# Product

A Product represents a something that can be purchased within the the Simple Store Platform.

The Product object comprises both a standard set of default fields along with a flexible model to extend the product to meet your customisation needs.

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
      <td style="text-align:left">A Url slug used to identify a product</td>
    </tr>
    <tr>
      <td style="text-align:left">Short Url</td>
      <td style="text-align:left">A globally unique id identrifier (see <a href="../getting-started/quickbuy.md">QuickBuy</a>)</td>
    </tr>
    <tr>
      <td style="text-align:left">Version</td>
      <td style="text-align:left">An incremental version number tracking changes to the Product configuration</td>
    </tr>
    <tr>
      <td style="text-align:left">Title</td>
      <td style="text-align:left">Default Title for the Product</td>
    </tr>
    <tr>
      <td style="text-align:left">Description</td>
      <td style="text-align:left">Default Description for the Product</td>
    </tr>
    <tr>
      <td style="text-align:left">Titles</td>
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
      <td style="text-align:left">Descriptions</td>
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
      <td style="text-align:left">IsActive</td>
      <td style="text-align:left">Active (True) or InActive (False)</td>
    </tr>
    <tr>
      <td style="text-align:left">Status</td>
      <td style="text-align:left">
        <p>Available = Product is Available</p>
        <p>Out Of Stock = Product is Out of Stock</p>
        <p>Discontinued = Product has been discontinued</p>
        <p>Unavailable = Product is unavailable</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Attributes</td>
      <td style="text-align:left">Attributes are a list of Key/Value to support customisation of a product</td>
    </tr>
    <tr>
      <td style="text-align:left">Categories</td>
      <td style="text-align:left">One or many categories the Product is assigned to (see <a href="categories.md">Categories</a>)</td>
    </tr>
    <tr>
      <td style="text-align:left">Collections</td>
      <td style="text-align:left">One or many collections the Product is assigned to (see <a href="collections.md">Collections</a>)</td>
    </tr>
    <tr>
      <td style="text-align:left">Files</td>
      <td style="text-align:left">One or many assets associated with the Product (see <a href="../assets-1/assets.md">Assets</a>)</td>
    </tr>
    <tr>
      <td style="text-align:left">Payment Method</td>
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
      <td style="text-align:left">BasePrice</td>
      <td style="text-align:left">See <a href="pricing.md">Pricing</a>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Price</td>
      <td style="text-align:left">See <a href="pricing.md">Pricing</a>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">BaseRewards</td>
      <td style="text-align:left">See <a href="rewards.md">Rewards </a>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Rewards</td>
      <td style="text-align:left">See <a href="rewards.md">Rewards </a>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Inventory</td>
      <td style="text-align:left">See <a href="inventory.md">Inventory</a>
      </td>
    </tr>
  </tbody>
</table>
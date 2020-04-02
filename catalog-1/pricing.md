# Pricing

Pricing of products comprise a specified base price and a dynamically calculated effective price.

![](../.gitbook/assets/image%20%2824%29.png)

### Base Price

The pricing information that has been assigned to the product itself via the console/api.

| Element | Description |
| :--- | :--- |
| CurrencyCode | ISO Currency code |
| SellPrice  | Is the advertised Price present to customer \(excluding specials, discounts or other modifiers\) |
| RetailPrice | Optional: Retail Price is the Recommended Retail Price \(RRP\)  |

### Effective Price

The effective price is the calculated price of the product after specials, discount or other modifiers have been applied to the product.  It is accessible as a read only property on the Catalog &gt; Product API Responses


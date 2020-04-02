# Rewards

Optionally the Simple Store platform supports rewards based pricing of products to support the purchase of product with points.

The rewards pricing of products comprises a specified base rewards price and a dynamically calculated effective rewards price.

![](../.gitbook/assets/image%20%2813%29.png)

### Base Rewards Pricing

The base rewards pricing in points that has been assigned to the product via the console/api.

| Element | Description |
| :--- | :--- |
| IsEnabled | Rewards pricing is enabled |
| Points | Product price in points |
| MinPayAmount | Minimum payment amount for purchase  |
| MinPointsAmount | Minimum points amount for purchase  |

### Effective Rewards

The effective rewards price is the calculated price in points of the product after specials, discounts or other modifiers have been applied to the product. It is accessible as read only properties on the Catalog &gt; Product API Responses


# Rewards

Optionally the Simple Store platform supports rewards based pricing of products to support the purchase of product with points.

The rewards pricing of products comprises a specified base rewards price and a dynamically calculated effective rewards price.

### Portal View

![](../.gitbook/assets/image%20%2823%29.png)

### Base Rewards Pricing Properties

The base rewards pricing in points that has been assigned to the product via the console/api.

{% tabs %}
{% tab title="Attributes" %}
| Element | Description |
| :--- | :--- |
| isEnabled | Rewards pricing is enabled |
| points | Product price in points |
| minPayAmount | Minimum payment amount for purchase  |
| minPointsAmount | Minimum points amount for purchase  |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
    "isEnabled":	boolean
    "points":	integer($int32)
    "minPayAmount":	number($decimal)
    "minPointsAmount":	number($decimal)
}
```
{% endtab %}
{% endtabs %}

### Effective Rewards

The effective rewards price is the calculated price in points of the product after specials, discounts or other modifiers have been applied to the product. It is accessible as read only properties on the Catalog &gt; Product API Responses


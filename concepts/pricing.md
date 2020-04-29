# Pricing

Pricing of products comprise a specified base price and a dynamically calculated effective price.

### Portal View

![](../.gitbook/assets/image%20%2854%29.png)

### Base Price

The pricing information that has been assigned to the product itself via the console/api.

{% tabs %}
{% tab title="Attributes" %}
| Element | Description |
| :--- | :--- |
| currencyCode | ISO Currency code |
| sellPrice  | Is the advertised Price present to customer \(excluding specials, discounts or other modifiers\) |
| retailPrice | Optional: Retail Price is the Recommended Retail Price \(RRP\)  |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
    "currencyCode":	"string"
    "sellPrice":	number($decimal)
    "retailPrice":	number($decimal)
    "attributes":	{...}
}
```
{% endtab %}
{% endtabs %}

### Effective Price

The effective price is the calculated price of the product after specials, discount or other modifiers have been applied to the product.  It is accessible as read only properties on the Catalog &gt; Product API Responses


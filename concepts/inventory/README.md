# Inventory

Optionally SimpleStore supports the tracking of product inventory.

### Portal View

![](../../.gitbook/assets/image%20%2825%29.png)

The following elements can be specified for management of inventory:

### Inventory Properties

{% tabs %}
{% tab title="Attributes" %}
| Element | Description |
| :--- | :--- |
| sku | Stock-keeping unit of product |
| availableQuantity | How many available in stock |
| minActiveQuantity | If AvailableQuantity is below this value then the Product will not longer will be available \(Status = Out Of Stock\) |
| grossWeight | Gross weight of the product |
| trackInventory | Enable tracking of inventory \(true\|false\) |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
    "sku":	"string"
    "availableQuantity":		number($double)
    "minActiveQuantity":		number($double)
    "grossWeight":		number($double)
    "trackInventory":		boolean
}
```
{% endtab %}
{% endtabs %}

|  |
| :--- |



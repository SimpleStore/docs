# Specials

Specials define rule based price modifiers to support discounting of products.

Specials can be either a **percentage** or a **fixed** amount.

Specials apply for a specified date range

Specials can be applied to:

* **Products** - specific products
* **Categories** - all Products assigned to a category
* **Collections** - all Products assigned to a collection

### Portal View

#### View Specials

Assess the **Special** screen in the console via the console navigation bar.

![](../.gitbook/assets/image%20%2812%29.png)

#### Add New Special

Click **Add New** to create a new special

![](../.gitbook/assets/image%20%2833%29.png)

Specified a:

* Name
* Description
* Special Type: Percentage or Fixed Amount
* Amount \(based on Special Type\)
* Date Range \(from and to\)

Click **Submit** to create the new special.

![](../.gitbook/assets/image%20%2824%29.png)

#### Edit Special 

Additional **Details** are specified including the definition of Rules that determined which products specials apply to.  Specials can apply to specific products or all products assigned to specifed Categories or Collections.

![](../.gitbook/assets/image%20%2841%29.png)

Click **Save** to commit your modifications.

#### Specials Properties

{% tabs %}
{% tab title="Attributes" %}
| Element | Description |
| :--- | :--- |
| specialId | Internal Identifier for the special |
| name | Name for the special |
| description | Description for the special |
| specialType | Percentage or Fixed Amount |
| amount | Amount of special, unit based on Special Type |
| startDate | Start date for the special |
| endDate | End date for the special |
| attributes | One or more key/value pairs to support customisation of specials |
| **Rules** |  |
| categories | Categories that the special applies to \(see [Categories](categories.md)\), if a Product is assigned to these categories then the special is applied |
| collections | Collections that the special applies to \(see [Specials](specials.md)\), if a Product is assigned to these collections then the special is applied |
| products | Products that the special applies to |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
    "specialId":	string
     "version	string
    "nullable: true
    "name	string
    "nullable: true
    "description	string
    nullable: true
    isActive	boolean
    startOnUtc	string($date-time)
    endOnUtc	string($date-time)
    nullable: true
    specialType	SpecialTypestring
    Enum:
    Array [ 2 ]
    amount	number($decimal)
    rules	[...]
    attributes	{...}
}
```
{% endtab %}
{% endtabs %}


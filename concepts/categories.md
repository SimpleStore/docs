# Categories

Products can be assigned to one or more categories which classify products into groups which could represent:

* Type of Product for example a "Toaster" category containing one or many Toasters.
* Products belonging to a special offer for example a "Special Deals" category contain one or many products with special pricing.
* Products assigned to be presented in a specific location within a channel, for example "Home Page Banner" for all products that are assigned to appear on a Banner on the Home Page of a website.

### Portal View

#### Accessing Categories 

Assess the **Categories** screen in the console via the console navigation bar.

![](../.gitbook/assets/image%20%2821%29.png)

#### Add New Category

Specified a Name for the category.

Click **New Category** to create the new category.

![](../.gitbook/assets/image%20%2838%29.png)

#### Edit Categories

Additional **Category Details** can be specified including:

![](../.gitbook/assets/image%20%284%29.png)

Click **Save** to commit your modifications.

### Category Properties

{% tabs %}
{% tab title="Attributes" %}
| Element | Description |
| :--- | :--- |
| categoryId | Internal Identifier for the category |
| name | Name of the category |
| slug | A Url slug to access the category |
| description | A Description for the category |
| attributes | One or more key/value pairs |
| parent Category | A parent category to support the creation of a hierarchical/tree based structure of related categories |
| images | Image \(assets\) assigned to a category |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "categoryId": "string",
  "version": "string",
  "slug": "string",
  "name": "string",
  "description": "string",
  "names": {
    "additionalProp1": "string",
    "additionalProp2": "string",
    "additionalProp3": "string"
  },
  "descriptions": {
    "additionalProp1": "string",
    "additionalProp2": "string",
    "additionalProp3": "string"
  },
  "parentId": "string",
  "parentName": "string",
  "itemCount": 0,
  "attributes": {},
  "children": [
    {
      "categoryId": "string",
      "name": "string",
      "slug": "string",
      "names": {
        "additionalProp1": "string",
        "additionalProp2": "string",
        "additionalProp3": "string"
      }
    }
  ],
  "totalChildren": 0,
  "sibling": [
    {
      "categoryId": "string",
      "name": "string",
      "slug": "string",
      "names": {
        "additionalProp1": "string",
        "additionalProp2": "string",
        "additionalProp3": "string"
      }
    }
  ],
  "totalSibling": 0,
  "isActive": true,
  "files": [
    {
      "fileId": "string",
      "contentType": "string",
      "accessPermission": "string",
      "accessUrl": "string",
      "attributes": {},
      "edgeUrl": "string"
    }
  ]
}
```
{% endtab %}
{% endtabs %}


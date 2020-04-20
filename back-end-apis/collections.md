# Collections

A collection represents a broad logical grouping of products.

Examples of collections could be:

* Winter Collection
* Premium Collection

### Portal View

#### View Collections

Assess the **Collection** screen in the console via the console navigation bar.

![](../.gitbook/assets/image%20%2834%29.png)



#### Add New Collection

Click **Add New** to create a new collection

![](../.gitbook/assets/image%20%285%29.png)

Specified a Name and Description for the collection.

Click **Submit** to create the new collection.

![](../.gitbook/assets/image.png)



#### Edit Collection

Additional **Collection Details** can be specified including:

![](../.gitbook/assets/image%20%2815%29.png)

Click **Save** to commit your modifications.

### Collection Properties

{% tabs %}
{% tab title="Attributes" %}
| Element | Description |
| :--- | :--- |
| collectionId | Internal Identifier for the collection |
| name | Name of the collection |
| slug | A Url slug to accese the collection |
| description | A Description for the collection |
| attributes | One or more key/value pairs |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "collectionId": "string",
  "version": "string",
  "name": "string",
  "slug": "string",
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
  "isActive": true,
  "totalItems": 0,
  "attributes": {}
}
```
{% endtab %}
{% endtabs %}



# Create Folder

Adds or updates a Product as an Item to the Cart.

The Cart Item is updated if the ProductId already exists in the Cart.  
  
Creates a Cart for a new cartId if a new CartId is provided.

If no CartId is provided a new Cart and CartId is created and the CartId is returned.

Carts are transient and expire after 14 days.

### **POST**

```text
/v1/folder/
```

#### Request: Route

No Route

#### Request: Query

No Query

#### Request:  Body

{% tabs %}
{% tab title="Request Object" %}
| Element | Type | Description |
| :--- | :--- | :--- |
| name | string | Folder Name |
| parentId | string | Unique Identifier for the Folder |
| attributes | object | Attributes are a list of Key/Value to support customisation of the folder items |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "currencyCode": "string",
  "items": [
    {
      "productId": "string",
      "quantity": 0
    }
  ],
  "attributes": {}
}
```
{% endtab %}
{% endtabs %}

#### Response: 201 Created

{% tabs %}
{% tab title="Response Object" %}
| Element | Type | Desciption |
| :--- | :--- | :--- |
| folderId | string |  |
| version | string |  |
{% endtab %}

{% tab title="Sample Object" %}
```text
"folderId": "string",
  "version": "string"
```
{% endtab %}
{% endtabs %}

#### Response: 404 Not Found

{% tabs %}
{% tab title="Response Object" %}
| Element | Type | Desciption |
| :--- | :--- | :--- |
| type | string |  |
| title | string |  |
| status | int |  |
| detail | string |  |
| instance | string |  |
| extensions | object |  |
{% endtab %}
{% endtabs %}


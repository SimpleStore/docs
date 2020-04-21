# Update Folder



Updates a folder‌

### **POST** <a id="post"></a>

```text
/v1/folder/{FolderId}
```

#### ‌Request: Route

| Element | Type | Description |
| :--- | :--- | :--- |
| FolderId | guid/uuid | A unique identifier for the cart |

#### Request: Query <a id="request-query"></a>

‌No Query‌

#### Request: Body <a id="request-body"></a>

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

#### Response: 200 Success

{% tabs %}
{% tab title="Response Object" %}
| Element | Type | Desciption |
| :--- | :--- | :--- |
| folderId | string |  |
| version | string |  |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
    "folderId": "string",
    "version": "string"
}
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


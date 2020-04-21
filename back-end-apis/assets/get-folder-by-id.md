# Get Folder By Id

Get Folder By Unique Folder Id

### **GET**

```text
/v1/folder/{FolderId}
```

#### Request: Route

| Element | Type | Description |
| :--- | :--- | :--- |
| FolderId | string | A unique identifier for the folder |

#### Response: 200 Ok

{% tabs %}
{% tab title="Response Object" %}
| Element | Type | Description |
| :--- | :--- | :--- |
| folderId | string | Unique Identifier for the Folder |
| version | string | incremental version number of folder object |
| name | string | Name |
| parentId | string | A parent folder identifier to support the creation of a hierarchical/tree based structure of related folder |
| attributes | object | Attributes are a list of Key/Value to support customisation of a folder |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "folderId": "string",
  "version": "string",
  "name": "string",
  "parentId": "string",
  "attributes": {}
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




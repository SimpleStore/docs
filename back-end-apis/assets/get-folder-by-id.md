# Get Folder By Id

Get Cart By Unique Cart Id

### **GET**

```text
/v1/folder/{FolderId}
```

#### Request: Route

| Element | Type | Description |
| :--- | :--- | :--- |
|  | guid/uuid | A unique identifier for the cart |

#### Response: 200 Ok

{% tabs %}
{% tab title="Response Object" %}
| Element | Type | Desciption |
| :--- | :--- | :--- |
| folderId | string |  |
| version | string |  |
|  |  |  |
|  |  |  |
|  |  |  |
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




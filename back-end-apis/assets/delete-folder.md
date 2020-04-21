# Delete Folder



Deletes a folder‌

### **DELETE** <a id="post"></a>

```text
/v1/folder/{FolderId}
```

#### ‌Request: Route

| Element | Type | Description |
| :--- | :--- | :--- |
| FolderId | string | A unique identifier for the folder |

#### Request: Query <a id="request-query"></a>

‌No Query‌

#### Request: Body <a id="request-body"></a>

No Body

#### Response: 200 Success

No Body

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


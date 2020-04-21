# Search Folders

Searches for Folders

### **GET**

```text
/v1/folders
```

#### Request: Route

No Route Values

#### Request: Query

| Element | Type | Description |
| :--- | :--- | :--- |
| Name | string | Folder Name |
| Attributes | object | Folder attributes |
| PageSize | integer | Page Size.  The number of records returned. |
| PageIndex | integer | Page Index.  The page of records returned. |

#### Request:  Body

No Request Body

#### Response: 200 Success



{% tabs %}
{% tab title="Response  Object" %}
| Element |  | Description |
| :--- | :--- | :--- |
| result | array | array of carts |
| result\[\].folderId | string | Unique Identifier for the Folder |
| result\[\].version | string | incremental version number of file object |
| result\[\].name | string | Name |
| result\[\].parentId | string | A parent folder identifier to support the creation of a hierarchical/tree based structure of related folder |
| pageSize | int | Page Size |
| pageIndex | int | Page Index |
| totalRecordsFound | int | Total Records Found |
| resultCount | int | Result Count |
| totalPages | int | Total Pages |
| queryDurationMilliseconds | int | Query Duration in Milliseconds |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "result": [
    {
      "folderId": "string",
      "version": "string",
      "name": "string",
      "parentId": "string"
     }
  ],
  "pageSize": 0,
  "pageIndex": 0,
  "totalRecordsFound": 0,
  "resultCount": 0,
  "totalPages": 0,
  "queryDurationMilliseconds": 0
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

{% tab title="Sample Object" %}
```text
{
  "type": "string",
  "title": "string",
  "status": 0,
  "detail": "string",
  "instance": "string",
  "extensions": {}
}
```
{% endtab %}
{% endtabs %}

#### 


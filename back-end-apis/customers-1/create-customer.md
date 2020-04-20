# Create Customer

Creates a Customer. 

### **POST**

```text
/v1/customers
```

#### Request: Route

No Route



#### Request: Query

No Query

#### Request: Body

{% tabs %}
{% tab title="Request Object" %}
| Element | Type | Description |
| :--- | :--- | :--- |
| firstName | string | First Name |
| lastName | string | Last Name |
| displayName | string | Display Name |
| emailAddress | string | Email Address |
| attributes | array | One or more key/value pairs to support customisation |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "firstName": "string",
  "lastName": "string",
  "displayName": "string",
  "emailAddress": "string",
  "attributes": {}
}
```
{% endtab %}
{% endtabs %}

#### Response: 201 Created

{% tabs %}
{% tab title="Response Object" %}


| Element | Type | Description |
| :--- | :--- | :--- |
| customerId | guid | Unique Customer Identifier |
| version | string | Incremental version number |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "customerId": "string",
  "version": "string"
}
```
{% endtab %}
{% endtabs %}

#### Response: 400 Bad Request

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


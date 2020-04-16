# Update Customer

Update a Customer by the Unique Customer Identifer. 

### **PUT**

```text
/v1/customers/{CustomerId}
```

#### Request: Route

| Element | Type | Description |
| :--- | :--- | :--- |
| Customer | guid/uuid | A unique identifier for the Customer |

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
{% endtabs %}


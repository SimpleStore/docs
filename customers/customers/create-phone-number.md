# Create Phone Number

Creates a Customer Phone Number. 

### **POST**

```text
/v1/customers/{CustomerId}/phones
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
| Element | Type | Desciption |
| :--- | :--- | :--- |
| Country | string | ISO Country Code |
| NumberLocal | string | Phone Number in Local format |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "country": "string",
  "numberLocal": "string"
}
```
{% endtab %}
{% endtabs %}

#### Response: 200 Success

{% tabs %}
{% tab title="Response Object" %}


| Element | Type | Description |
| :--- | :--- | :--- |
| customerId | guid | Unique Customer Identifier |
| version | string | Incremental version number |
| totalPhonesAttached | int | Count of Total Phone Number |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "customerId": "string",
  "version": "string",
  "totalPhonesAttached": 0
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


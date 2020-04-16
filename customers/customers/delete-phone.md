# Delete Phone Number

Delete one or many Customer Phone Numbers. 

### **DELETE**

```text
/v1/customers/{CustomerId}/phones
```

#### Request: Route

| Element | Type | Description |
| :--- | :--- | :--- |
| Customer | guid/uuid | A unique identifier for the Customer |

#### Request: Query

| Element | Type | Description |
| :--- | :--- | :--- |
| Version | string | Version Number |

#### Request: Body

{% tabs %}
{% tab title="Request Object" %}
| Element | Type | Desciption |
| :--- | :--- | :--- |
| keys | array | Array of Keysode |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "keys": [
    "string"
  ]
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
| phonesRemoved | array | Array of phone numbers removed |
| phonesRemoved\[\].key | string | A unique identifier for the Phone Number \(Guid/UUID\) |
| phonesRemoved\[\].type | string | Unknown, Phone, Mobile |
| phonesRemoved\[\].country | string | ISO Country Code |
| phonesRemoved\[\].numberLocal | string | Phone Number in Local format |
| phonesRemoved\[\].numberInternational | string | Phone Number in International format |
| totalPhonesAttached | int | Count of Total Phone Number |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "customerId": "string",
  "version": "string",
  "phonesRemoved": [
    {
      "key": "string",
      "type": "Unknown",
      "country": "string",
      "numberLocal": "string",
      "numberInternational": "string"
    }
  ],
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


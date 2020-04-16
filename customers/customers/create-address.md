# Create Address



Creates a Customer Address. 

### **POST**

```text
/v1/customers/{CustomerId}/addresses
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
| Address1 | string | Address Line 1 |
| Address2 | string | Address Line 2 |
| Suburb | string | Suburb |
| PostCode | string | Postal Code/Zip Code |
| State | string | State/Province/Region |
| Country | string | Country |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "address1": "string",
  "address2": "string",
  "suburb": "string",
  "postcode": "string",
  "state": "string",
  "country": "string"
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
| totalAddressesAttached | int | Count of Total Addresses |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "customerId": "string",
  "version": "string",
  "totalAddressesAttached": 0
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


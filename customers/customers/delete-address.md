# Delete Address

Delete one or many Customer Addresses. 

### **DELETE**

```text
/v1/customers/{CustomerId}/addresses
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
| keys | array | Array of Address Keys |
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
| addressesRemoved | array | Array of phone numbers removed |
| addressesRemoved\[\].key | string | A unique identifier for the Phone Number \(Guid/UUID\) |
| addressesRemoved\[\].address1 | string | Address Line 1 |
| addressesRemoved\[\].address2 | string | Address Line 2 |
| addressesRemoved\[\].suburb | string | Suburb |
| addressesRemoved\[\].postcode | string | Postal Code/Zip Code |
| addressesRemoved\[\].state | string | State/Province/Region |
| addressesRemoved\[\].country | string | Country |
| totalAddressesAttached | int | Count of Total Addresses |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "customerId": "string",
  "version": "string",
  "addressesRemoved": [
    {
      "key": "string",
      "address1": "string",
      "address2": "string",
      "suburb": "string",
      "postcode": "string",
      "state": "string",
      "country": "string"
    }
  ],
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


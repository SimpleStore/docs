# Search Customers

Search for one or many Customers. 

### **GET**

```text
/v1/customers
```

#### Request: Route

No Route

#### Request: Query

{% tabs %}
{% tab title="Request Object" %}
| Element | Type | Description |
| :--- | :--- | :--- |
| CustomerId | array | An array of CustomerIds |
| EmailAddress | string | Email Address |
| IncludePhones | bool | Display Name |
| IncludeAddresses | bool | Include Addresses in Result |
| IncludeAttributes | bool | Include Attributes in Result |
| Attributes | objects |  |
| PageSize | int | Page Size.  The number of records returned. |
| PageIndex | int  | Page Index.  The page of records returned. |
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

#### Response: 200 Success

{% tabs %}
{% tab title="Response Object" %}


| Element | Type | Desciption |
| :--- | :--- | :--- |
| result | array | array of customers |
| result\[\].customerId | guid | A unique identifier for the Customer \(Guid/UUID\) |
| result\[\].version | string | A incremental version number tracking modifications to the Customer object |
| result\[\].firstName | string | Customer First Name |
| result\[\].lastName | string | Customer Last Name |
| result\[\].displayName | string | Customer Display Name |
| result\[\].emailAddress | string | Customer Email Address in  |
| result\[\].phones\[\] | array | An array of Phone numbers |
| result\[\].phones\[\].Key | guid | A unique identifier for the Phone Number \(Guid/UUID\) |
| result\[\].phones\[\].Type | string | Unknown, Phone, Mobile |
| result\[\].phones\[\].Country | string | ISO Country Code |
| result\[\].phones\[\].NumberLocal | string | Phone Number in Local format |
| result\[\].phones\[\].NumberInternational | string | Phone Number in International format |
| result\[\].addresses\[\] | array | An array of address\(es\) |
| result\[\].addresses\[\].Key | guid | A unique identifier for the Address \(Guid/UUID\) |
| result\[\].addresses\[\].Address1 | string | Address Line 1 |
| result\[\].addresses\[\].Address2 | string | Address Line 2 |
| result\[\].addresses\[\].Suburb | string | Suburb |
| result\[\].addresses\[\].PostCode | string | Postal Code/Zip Code |
| result\[\].addresses\[\].State | string | State/Province/Region |
| result\[\].addresses\[\].Country | string | Country |
| result\[\].attributes | object | Attributes are a list of Key/Value to support customisation of a Customer |
| pageSize | int | Page Size |
| pageIndex | int | Page Index  |
| totalRecordsFound | int | Total Records Found |
| resultCount | int | Result Count |
| totalPages | int | Total Pages  |
| queryDurationMilliseconds | int | Query Duration in Milliseconds |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "result": [
    {
      "customerId": "string",
      "version": "string",
      "firstName": "string",
      "lastName": "string",
      "displayName": "string",
      "emailAddress": "string",
      "phones": [
        {
          "key": "string",
          "type": "Unknown",
          "country": "string",
          "numberLocal": "string",
          "numberInternational": "string"
        }
      ],
      "addresses": [
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
      "attributes": {}
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


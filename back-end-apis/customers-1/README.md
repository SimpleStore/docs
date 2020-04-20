# Customers

The Customer object supports the storage of a defined set and custom attributes relating to your customers.

{% tabs %}
{% tab title="Attributes" %}
| Element | Description |
| :--- | :--- |
| customerId | A unique identifier for the Customer \(Guid/UUID\) |
| version | A incremental version number tracking modifications to the Customer object |
| firstName | Customer First Name |
| lastName | Customer Last Name |
| displayName | Customer Display Name |
| emailAddress | Customer Email Address in  |
| phones\[\] | An array of Phone numbers |
| phones\[\].Key | A unique identifier for the Phone Number \(Guid/UUID\) |
| phones\[\].Type | Unknown, Phone, Mobile |
| phones\[\].Country | ISO Country Code |
| phones\[\].NumberLocal | Phone Number in Local format |
| phones\[\].NumberInternational | Phone Number in International format |
| addresses\[\] | An array of address\(es\) |
| addresses\[\].Key | A unique identifier for the Address \(Guid/UUID\) |
| addresses\[\].Address1 | Address Line 1 |
| addresses\[\].Address2 | Address Line 2 |
| addresses\[\].Suburb | Suburb |
| addresses\[\].PostCode | Postal Code/Zip Code |
| addresses\[\].State | State/Province/Region |
| addresses\[\].Country | Country |
| attributes | Attributes are a list of Key/Value to support customisation of a Customer |
{% endtab %}

{% tab title="Sample Object" %}
```text
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
```
{% endtab %}
{% endtabs %}


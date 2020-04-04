# Customers

The Customer object supports the storage of a defined set and custom attributes relating to your customers.

{% tabs %}
{% tab title="Attributes" %}
| Element | Description |
| :--- | :--- |
| CustomerId | A unique identifier for the Customer \(Guid/UUID\) |
| Version | A incremental version number tracking modifications to the Customer object |
| FirstName | Customer First Name |
| LastName | Customer Last Name |
| DisplayName | Customer Display Name |
| EmailAddress | Customer Email Address in  |
| Phones\[\] | An array of Phone numbers |
| Phone.Key | A unique identifier for the Phone Number \(Guid/UUID\) |
| Phone.Type | Unknown, Phone, Mobile |
| Phone.Country | ISO Country Code |
| Phone.NumberLocal | Phone Number in Local format |
| Phone.NumberInternational | Phone Number in International format |
| Addresses\[\] | An array of Addresses |
| Address.Key | A unique identifier for the Address \(Guid/UUID\) |
| Address.Address1 | Address Line 1 |
| Address.Address2 | Address Line 2 |
| Address.Suburb | Suburb |
| Address.PostCode | Postal Code/Zip Code |
| Address.State | State/Province/Region |
| Address.Country | Country |
| Attributes | Attributes are a list of Key/Value to support customisation of a Customer |
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


# Delete Customer



Deleted a Customer by the Unique Customer Identifer. 

### **DELETE**

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

No Body

#### Response: 200 Success

No Response Body

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


# Orders

The Order object stores completed Orders.

### Portal View

#### Accessing Orders

Assess the Orders screen in the console via the console navigation bar.

![](../.gitbook/assets/image%20%2832%29.png)

#### 

#### View Orders

Orders can be accessed by clicking on the main order screen:

![](../.gitbook/assets/image%20%2828%29.png)

Click **Save** to commit your modifications.

Customers can be deleted by clicking the **Delete** button.

### Order Properties

{% tabs %}
{% tab title="Attributes" %}
| Element | Description |
| :--- | :--- |
| orderId | A unique identifier for the Order \(Guid/UUID\) |
| version | A incremental version number tracking modifications to the Customer object |
| status | The Order Status \(\) |
| createdOnUtc | Created in UTC time \(2020-04-29T10:02:03.212Z\) |
| customerId | A unique identifier for the Customer \(Guid/UUID\) |
| purchaserName | Purchaser Name |
| purchaserContactNumberLocal | Purchaser Contact Number \(local\) |
| purchaserEmail | Purchaser Email Address |
| receiverName | Receiver Name  |
| receiverContactNumberLocal | Receiver Contact Number \(local\) |
| receiverEmail | Receiver Email Address |
| items\[\] | An array of Items |
| items\[\].productId | A unique identifier for the Product \(Guid/UUID\) |
| items\[\].quantity | Quantity of Product |
| items\[\].sellPrice | Sell Price |
| items\[\].total | Total \(Quantity x Sell Price\) |
| currencyCode | ISO currency code |
| shippingFee | Shipping Fee |
| subtotal | Total \(excluding Shipping Fee\) |
| total | Total |
| payments\[\] | An array of payments |
| payments\[\].paymentId | A unique identifier for the Payment \(Guid/UUID\) |
| payments\[\].paidOnUtc | Paid in UTC time \(2020-04-29T10:02:03.212Z\) |
| payments\[\].type | Payment Type \(Credit, Cash, Points\) |
| payments\[\].status | Payment Status |
| payments\[\].paidAmount | Payment Amount |
| payments\[\].cancellationReason | Cancellation Reason |
| payments\[\].refundId | Redund Identifier |
| payments\[\].refundReason | Redund Reason |
| payments\[\].attributes | Attributes are a list of Key/Value to support customisation of a Payment |
| totalPaid | Total Paid \(Total of all Payments\) |
| attributes | Attributes are a list of Key/Value to support customisation of a Order |
{% endtab %}

{% tab title="Sample Object" %}
```text
{
  "orderId": "string",
  "version": "string",
  "status": "Created",
  "createdOnUtc": "2020-04-29T10:02:03.212Z",
  "customerId": "string",
  "purchaserName": "string",
  "purchaserContactNumberLocal": "string",
  "purchaserEmail": "string",
  "receiverName": "string",
  "receiverContactNumberLocal": "string",
  "receiverEmail": "string",
  "items": [
    {
      "productId": "string",
      "title": "string",
      "quantity": 0,
      "sellPrice": 0,
      "total": 0
    }
  ],
  "currencyCode": "string",
  "shippingFee": 0,
  "subtotal": 0,
  "total": 0,
  "payments": [
    {
      "paymentId": "string",
      "paidOnUtc": "2020-04-29T10:02:03.212Z",
      "type": "Credit",
      "status": "Successful",
      "paidAmount": 0,
      "cancellationReason": "string",
      "refundId": "string",
      "refundReason": "string",
      "attributes": {}
    }
  ],
  "totalPaid": 0,
  "attributes": {}
}
```
{% endtab %}
{% endtabs %}


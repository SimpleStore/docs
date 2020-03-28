# Pagination

Pagination is used in all API endpoints that return a list of results.

**Example:**

```javascript
{
    "result": [],
    "pageSize": 10,
    "pageIndex": 0,
    "totalRecordsFound": 0,
    "resultCount": 0,
    "totalPages": 0,
    "queryDurationMilliseconds": 48
}
```

Each response will contain paging information alongside the results. To change pages or the page size, when making the GET request, append the following Query Parameters   `?pageSize=10&pageIndex=1`

{% hint style="info" %}
If no paging parameter are provided, default values are used. `pageSize=10&pageIndex=0`
{% endhint %}


![](https://s3.eu-west-2.amazonaws.com/cdn.debtpanel.co.uk/images/green-white.jpg)

# DebtPanel - Referral Guide

## Summary Object

The basic Summary Object that is posted will comprise of the following properties.

### Example Object

``` json
{
    "creditors": 4139495,
    "income": 370000,
    "expenditure": 347268,
    "disposableIncome": 22731
}
```

### Property Guide

:warning: **Please Note:** All monetary values are sent in pennies by default, to find the pound and pence value you would have to divide the figure by 100.

Property | Type | Description
--- | --- | ---
creditors | Integer | An integer storing the total value of outstanding debt to all creditors
income | Integer | An integer storing the total income from all income sources
expenditure | Integer | An integer storing the total expenditure from all expenditure sources
disposableIncome | Integer | An integer storing the disposable income for the client, found by subtracting total expenditure from total income

### Extra Available properties

On request we are able to include the following properties inside this object.

Property | Type | Description
--- | --- | ---
properties | Integer | An integer containing the total value of all properties owned by the client
vehicles | Integer | An integer containing the total value of all vehicles owned by the client
assets | Integer | An integer containing the total value of all assets owned by the client

### Available Transformations

On request we are able to apply the following transformations to given properties.

Property | Standard Type | Transformed Type | Standard Example | Transformed Example
--- | --- | --- | --- | ---
creditors | Integer | Float<br />String | 4139495 | 41394.95<br />"£41,394.95"
income | Integer | Float<br />String | 370000 | 3700.00<br />"£3,700.00"
expenditure | Integer | Float<br />String | 347268 | 3472.68<br />"£3,472.68"
disposableIncome | Integer | Float<br />String | 22731 | 227.31<br />"£227.31"
properties | Integer | Float<br />String | 4139495 | 41394.95<br />"£41,394.95"
vehicles | Integer | Float<br />String | 4139495 | 41394.95<br />"£41,394.95"
assets | Integer | Float<br />String | 4139495 | 41394.95<br />"£41,394.95"


#### Quick Links

[:arrow_backward:](client.md) [:information_source:](../readme.md)
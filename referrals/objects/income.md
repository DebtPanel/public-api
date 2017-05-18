# DebtPanel - Referral Guide

## Income Object

The basic Income Object that is posted will comprise of the following properties.

### Example Object

``` json
{
    "name": "Client Wage",
    "value": 169900,
    "note": "A Note Goes Here"
}
```

### Property Guide

:warning: **Please Note:** All monetary values are sent in pennies by default, to find the pound and pence value you would have to divide the figure by 100.

Property | Type | Description
--- | --- | ---
name | String(255)[`<IncomeType>`](../types/income.md) | A string containing the type of income this refers to
value | Integer | An integer storing the amount spent on this income item
note | String(4096) | A string containing an important note about this income item

### Extra Available properties

On request we are able to include the following properties inside this object.

Property | Type | Description
--- | --- | ---
id | String(24) | This ID references the income type and is not specific to client so it can be used to match against income items in the external system.<br />**Example:** `"id": "f98585ec53d7ec45554aa80f"`

### Available Transformations

On request we are able to apply the following transformations to given properties.

Property | Standard Type | Transformed Type | Standard Example | Transformed Example
--- | --- | --- | --- | ---
value | Integer | Float<br />String | 169900 | 1699.00<br />"£1,699.00"

We are also able to transform the DebtPanel ID property into an ID that matches a unique identifier in the External system if you send us a guide as to which DebtPanel ID's relate to ID's in the external system.

Property | Standard Type | Transformed Type | Standard Example | Transformed Example
--- | --- | --- | --- | ---
id | String(24) | Integer | "f98585ec53d7ec45554aa80f" | 37

#### Quick Links

[:arrow_backward:](client.md) [:information_source:](../readme.md)
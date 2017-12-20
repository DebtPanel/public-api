# DebtPanel - Referral Guide

## Creditor Object

The basic Creditor Object that is posted will comprise of the following properties.

### Example Object

``` json
{
    "reference": "92888371-bg",
    "type": "Pay Day Loans",
    "secured": false,
    "creditor": "AtoB Loans Inc",
    "owner": "client",
    "value": 812095,
    "status": "active",
    "note": null
}
```

### Property Guide

:warning: **Please Note:** All monetary values are sent in pennies by default, to find the pound and pence value you would have to divide the figure by 100.

Property | Type | Description
--- | --- | ---
reference | String(40) | A string containing the account number of the account at the creditor
type | String(150)[`<CreditorType>`](../types/creditor.md) | A string containing the type of creditor this refers to
secured | Boolean | A boolean value showing if the credit is secured or not
creditor | String(255) | A string containing the name of the creditor
owner | String(10) | The owner of the credit. Can be either client, partner or joint
value | Integer | An integer storing the amount spent on this creditor item
status | String(20) | A string containing the status of the credit. Can be Active, Defaulted or Closed
note | String(4096) | A string containing an important note about this creditor item

### Extra Available properties

On request we are able to include the following properties inside this object.

Property | Type | Description
--- | --- | ---
id | String(24) | This ID references the creditor type and is not specific to client so it can be used to match against creditor items in the external system.<br />**Example:** `"id": "f98585ec53d7ec45554aa80f"`
source | String(125) | A string containing how the information was obtained. Can be either 'Manual Input' or 'Credit Check'


### Available Transformations

On request we are able to apply the following transformations to given properties.

Property | Standard Type | Transformed Type | Standard Example | Transformed Example
--- | --- | --- | --- | ---
value | Integer | Float<br />String | 812095 | 8120.95<br />"£8,120.95"

We are also able to transform the DebtPanel ID property into an ID that matches a unique identifier in the External system if you send us a guide as to which DebtPanel ID's relate to ID's in the external system.

Property | Standard Type | Transformed Type | Standard Example | Transformed Example
--- | --- | --- | --- | ---
id | String(24) | Integer | "f98585ec53d7ec45554aa80f" | 37

#### Quick Links

[Back](client.md) [Home](../readme.md)

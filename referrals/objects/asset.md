# DebtPanel - Referral Guide

## Asset Object

The basic Asset Object that is posted will comprise of the following properties.

### Example Object

``` json
{
    "type": "Cash at Bank",
    "value": 765000,
    "owner": "client",
    "note": ""
}
```

### Property Guide

:warning: **Please Note:** All monetary values are sent in pennies by default, to find the pound and pence value you would have to divide the figure by 100.

Property | Type | Description
--- | --- | ---
type | String(255)[`<AssetType>`](../types/asset.md) | A string containing the type of asset this refers to
value | Integer | An integer storing the amount spent on this asset item
owner | String(10) | The owner of the asset. Can be either client, partner or joint
note | String(4096) | A string containing an important note about this asset item

### Extra Available properties

On request we are able to include the following properties inside this object.

Property | Type | Description
--- | --- | ---
id | String(24) | This ID references the asset type and is not specific to client so it can be used to match against asset items in the external system.<br />**Example:** `"id": "f98585ec53d7ec45554aa80f"`

### Available Transformations

On request we are able to apply the following transformations to given properties.

Property | Standard Type | Transformed Type | Standard Example | Transformed Example
--- | --- | --- | --- | ---
value | Integer | Float<br />String | 6599 | 65.99<br />"£65.99"

We are also able to transform the DebtPanel ID property into an ID that matches a unique identifier in the External system if you send us a guide as to which DebtPanel ID's relate to ID's in the external system.

Property | Standard Type | Transformed Type | Standard Example | Transformed Example
--- | --- | --- | --- | ---
id | String(24) | Integer | "f98585ec53d7ec45554aa80f" | 37

#### Quick Links

[Back](client.md) [Home](../readme.md)

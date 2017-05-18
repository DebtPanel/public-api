# DebtPanel - Referral Guide

## Property Object

The basic Property Object that is posted will comprise of the following properties.

### Example Object

``` json
{
    "address1": "123 Test Road",
    "address2": null,
    "address3": null,
    "town": "TesterTon",
    "county": "TestVille",
    "postalCode": "TE7 5ER",
    "propertyType": "Detached House",
    "years": 8,
    "months": 7,
    "note": "Buy To Let",
    "value": 11200000,
    "owner": "joint"
}
```

### Property Guide

:warning: **Please Note:** All monetary values are sent in pennies by default, to find the pound and pence value you would have to divide the figure by 100.

Property | Type | Description
--- | --- | ---
address1 | String(255) | A string containing first address line of the property
address2 | String(255) | A string containing second address line of the property
address3 | String(255) | A string containing third address line of the property
town | String(150) | A string containing the town of the property
county | String(100) | A string containing the county of the property
postalCode | String(12) | A string containing the postcode of the property
propertyType | String(100)[`<PropertyType>`](../types/property.md) | A string containing the type of property
years | Integer | An integer showing how many years the property has been owned for
months | Integer | An integer showing how many months the property has been owned for
note | String(4096) | A string containing an important note about this property item
value | Integer | An integer storing the amount spent on this property item
owner | String(10) | The owner of the property. Can be either client, partner or joint

### Available Transformations

On request we are able to apply the following transformations to given properties.

Property | Standard Type | Transformed Type | Standard Example | Transformed Example
--- | --- | --- | --- | ---
value | Integer | Float<br />String | 6599 | 65.99<br />"£65.99"

We are also able to transform the DebtPanel propertyType into an ID that matches a unique identifier in the External system if you send us a guide as to which DebtPanel propertyType's relate to ID's in the external system.

Property | Standard Type | Transformed Type | Standard Example | Transformed Example
--- | --- | --- | --- | ---
propertyType | String(100) | Integer | "Detached House" | 4
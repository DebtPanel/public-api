![](https://s3.eu-west-2.amazonaws.com/cdn.debtpanel.co.uk/images/green-white.jpg)

# DebtPanel - Referral Guide

## Vehicle Object

The basic Vehicle Object that is posted will comprise of the following properties.

### Example Object

``` json
{
    "registration": "S33 CLX",
    "make": "Ford",
    "model": "Focus",
    "year": "2006",
    "value": 120000,
    "owner": "partner",
    "note": "Car"
}
```

### Property Guide

:warning: **Please Note:** All monetary values are sent in pennies by default, to find the pound and pence value you would have to divide the figure by 100.

Property | Type | Description
--- | --- | ---
registration | String(10) | A string containing the vehicle registration number
make | String(100) | A string make of the vehicle
model | String(100) | A string model of the vehicle
year | String(4) | A string containing year the vehicle was registered in
value | Integer | An integer storing the amount the vehicle is currently worth
owner | String(10) | The owner of the asset. Can be either client, partner or joint
note | String(4096) | A string containing an important note about this vehicle

### Available Transformations

On request we are able to apply the following transformations to given properties.

Property | Standard Type | Transformed Type | Standard Example | Transformed Example
--- | --- | --- | --- | ---
year | String | Integer | "2006" | 2006
value | Integer | Float<br />String | 6599 | 65.99<br />"£65.99"


#### Quick Links

[:arrow_backward:](client.md) [:information_source:](../readme.md)
# DebtPanel - Referral Guide

## Address Object

The basic Address Object that is posted will comprise of the following properties.

### Example Object

``` json
{
    "address1": "Test",
    "address2": null,
    "address3": null,
    "town": "test",
    "county": "test",
    "postalCode": "TE5 7ER",
}
```

### Property Guide

Property | Type | Description
--- | --- | ---
address1 | String(255) | A string containing first address line of the address
address2 | String(255) | A string containing second address line of the address
address3 | String(255) | A string containing third address line of the address
town | String(150) | A string containing the town of the address
county | String(100) | A string containing the county of the address
postalCode | String(12) | A string containing the postcode of the address
postalCode | String(12) | A string containing the postcode of the address

### Extra Available properties

On request we are able to include the following properties inside this object.

Property | Type | Description
--- | --- | ---
country | String(50) | A string containing the country of the address

#### Quick Links

[Back](person.md) [Home](../readme.md)

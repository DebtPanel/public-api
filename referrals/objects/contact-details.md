# DebtPanel - Referral Guide

## Contact Details Object

The basic Contact Details Object that is posted will comprise of the following properties.

### Example Object

``` json
{
    "landline": "01204297397",
    "mobile": "07457889465",
    "email": "c.skinner.86@gmail.com"
}
```

### Property Guide

Property | Type | Description
--- | --- | ---
landline | String(11) | A string storing the landline number
mobile | String(11) | A string storing the mobile number
email | String(255) | A string storing the email address

### Available Transformations

On request we are able to apply the following transformations to given properties.

Property | Standard Type | Transformed Type | Standard Example | Transformed Example
--- | --- | --- | --- | ---
landline | String(11) | String(12)<br />String(13) | "01204297397" | "441204297397"<br />"+441204297397"
mobile | String(11) | String(12)<br />String(13) | "07457889465" | "447457889465"<br />"+447457889465"

#### Quick Links

[Back](person.md) [Home](../readme.md)

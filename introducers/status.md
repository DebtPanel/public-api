![](https://s3.eu-west-2.amazonaws.com/cdn.debtpanel.co.uk/images/green-white.jpg)

# DebtPanel - Introducer Guide

## Status

This route enables the person calling it check that our API is active.

### Endpoint and Method

`GET` https://api.debtpanel.co.uk/status

### Parameters

No parameters are required for this route.

### Responses

Code | Description | Object
---- | ----------- | ------
200 | API is working correctly | [ApiStatus](#apiStatus)
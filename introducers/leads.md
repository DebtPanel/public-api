![](https://s3.eu-west-2.amazonaws.com/cdn.debtpanel.co.uk/images/green-white.jpg)

# DebtPanel - Introducer Guide

## Leads

This route enables the person calling it check that our API is active.

### Security

This route is protected by API key security, one must be supplied in the header
to enable leads to be passed. Please see the [security](security.md) document
for more information.

### Endpoint and Method

`POST` https://api.debtpanel.co.uk/leads

### Parameters

Name | Located in | Description | Required | Object
---- | ---------- | ----------- | -------- | ----
body | body | Main Lead to add | Yes | [Submission](objects/submission.md)

### Responses

Code | Description | Object
---- | ----------- | ------
201 | Item created | [LeadResponse](#leadResponse)
400 | Invalid input, object invalid | [Error400](#error400)
401 | API key not provided | [Error401](#error401)
403 | API key provided but is not valid | [Error403](#error403)
409 | An existing item already exists | [Error409](#error409)
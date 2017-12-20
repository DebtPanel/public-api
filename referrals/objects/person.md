# DebtPanel - Referral Guide

## Person Object

The basic Person Object that is posted will comprise of the following properties.

### Example Object

```json
{
    "title": "Mrs",
    "firstName": "Claire",
    "middleNames": null,
    "lastName": "Skinner",
    "maidenName": "Bradshaw",
    "dateOfBirth": "1986-12-17",
    "gender": "F",
    "address": { },
    "contactDetails": { },
    "maritalStatus": "Married",
    "residentialStatus": "Tenant - Private",
    "employmentStatus": "Employed",
    "occupation": "Barmaid",
    "employer": "Wetherspoons"
}
```

### Property Guide

Property | Type | Description
--- | --- | ---
title | String(25)[`<Title>`](../types/title.md) | A string storing the title of the person
firstName | String(100) | A string storing the first name of the person
middleNames | String(200) | A string storing all middle names of the person (Separated by a space)
lastName | String(100) | A string storing the last name of the person
maidenName | String(100) | A string storing the maiden name of the person
dateOfBirth | String(10) | A string holding the date of birth of the person in international format (YYYY-MM-DD)
gender | String(1) | An single character string storing the gender of the person. Can be 'M', 'F' or null.
address | Object[`<Address>`](address.md) | An integer storing the total value of outstanding debt to all creditors
maritalStatus | String(100)[`<MaritalStatus>`](../types/marital-status.md) | A string storing the marital status of the person
contactDetails | Object[`<ContactDetails>`](contact-details.md) | An integer storing the total value of outstanding debt to all creditors
residentialStatus | String(100)[`<ResidentialStatusType>`](../types/residential-status.md) | A string storing the residential status of the person
employmentStatus | String(100)[`<EmploymentStatusType>`](../types/employment-status.md) | A string storing the employment status of the person
occupation | String(200) | A string storing the occupation of the person
employer | String(255) | A string storing the name of the person's employer


#### Quick Links

[Back](client.md) [Home](../readme.md)

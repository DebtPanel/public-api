![](https://s3.eu-west-2.amazonaws.com/cdn.debtpanel.co.uk/images/green-white.jpg)

# DebtPanel - Introducer Guide

## Introduction

This introducer guide aims to help any introducers understand the API that can be used
to send in

## Contents

### Example Code

Document | Description
-------- | -----------
[JSON Example](example.json) | A full json string showing all fields that we pass by default

### Objects

Document | Description
-------- | -----------
[Base Structure](objects/client.md) | The basic breakdown of the object we post to external systems
[Person](objects/person.md) | This object holds the details of a person which will be used for a Client or a Partner
[Address](objects/address.md) | This object will hold a standard postal address
[ContactDetails](objects/contact-details.md) | This object holds contact details such as phone numbers and email address
[Dependant](objects/dependant.md) | This object stores a count and date of births of dependants
[Creditor](objects/creditor.md) | This object holds the details of a creditor
[Property](objects/property.md) | This object holds the details of a property owned by the client
[Vehicle](objects/vehicle.md) | This object holds details of vehicles owned by the client
[Asset](objects/asset.md) | This object stores details of any assets held by the client
[Income](objects/income.md) | This object holds details of any income the client has
[Expenditure](objects/expenditure.md) | This object holds details of any expenditure the client has
[Summary](objects/summary.md) | This object holds a basic financial summary of the client

### Types

The standard default JSON structure we post to external systems converts all of the types in
DebtPanel into static text strings. However, we can add the DebtPanel ID to most objects and
can also transform these to Integer IDs that match your system.

To help manage these we have created a list of all converted types, and include the DebtPanel
ID for each of these so that External systems can handle them appropriately.

Document | Description
-------- | -----------
[Residential Status](types/residential-status.md) | The residential status of a person. e.g. 'Living With Parents'
[Employment Status](types/employment-status.md) | The employment status of a person. e.g. 'Self Employed'
[Creditor](types/creditor.md) | The type of creditor that is listed. e.g. 'Pay Day Loan'
[Property](types/property.md) | The type of property owned. e.g. 'Semi-Detached'
[Asset](types/asset.md) | The type of asset owned. e.g. 'Pension'
[Income](types/income.md) | The type of income that is earned. e.g. 'Salary'
[Expenditure](types/expenditure.md) | The type of expenditure. e.g. 'Mobile Phone Contract'

#### Quick Links

[:information_source:](../readme.md)
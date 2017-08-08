# DebtPanel - Referral Guide

## Client Object

The basic Client Object that is posted will comprise of the following properties.

### Example Object

``` json
{
  "reference": "",
  "client": {  },
  "partner": {  },
  "dependants": {  },
  "creditors": [  ],
  "properties": [  ],
  "vehicles": [  ],
  "assets": [  ],
  "income": [  ],
  "expenditure": [  ],
  "summary": {  }
}
```

### Property Guide

Property | Type | Description
--- | --- | ---
reference | String`(24)` | Holds the DebtPanel reference for this client which will be required for any communication back to DebtPanel
client | Object[`<Person>`](person.md) | A Person object holding all details of the main client being submitted
partner | Object[`<Person>`](person.md) | A Person object holding all details of the partner of the client being submitted
dependants | Object[`<Dependant>`](dependant.md) | A Dependant object holding a count and Dates of Birth for any dependants under 18 years old
creditors | Array[`<Creditor>`](creditor.md) | An array of Creditor objects showing each creditor the client owes money to and the status of that creditor
properties | Array[`<Property>`](property.md) | An array of Property objects showing all properties owned by the client
vehicles | Array[`<Vehicle>`](vehicle.md) | An array of Vehicle objects showing all vehicles owned by the client
assets | Array[`<Asset>`](asset.md) | An array of Asset objects showing any assets the client may have that are not already listed in other categories
income | Array[`<Income>`](income.md) | An array of Income objects showing all Income the client has
expenditure | Array[`<Expenditure>`](expenditure.md) | An array of Expenditure objects showing all Expenditure the client has
summary | Object[`<Summary>`](summary.md) | A Summary object showing a brief summary of the client's Income, Expenditure, Creditors and Disposable Income


#### Quick Links

[Home](../readme.md)

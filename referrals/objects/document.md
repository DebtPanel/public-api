# DebtPanel - Referral Guide

## Document Object

The basic Document Object that is posted will comprise of the following properties.

### Example Object

``` json
{
  "type": "Bank Statements",
  "documentLink": "bank-statement-bank-statement.txt",
  "encodedDocument": "QmFuayBTdGF0ZW1lbnQ="
}
```

### Property Guide

Property | Type | Description
--- | --- | ---
type | String(150)[`<DocumentType>`](../types/document.md) | A string containing the type of document this refers to
documentLink | String(250) | A string showing the filename of the document being transferred
encodedDocument | Text | A text field containing a base64 encoded version of the file being sent.

### Extra Available properties

On request we are able to include the following properties inside this object.

Property | Type | Description
--- | --- | ---
id | String(24) | This ID references the document type and is not specific to client so it can be used to match against document types in the external system.<br />**Example:** `"id": "f98585ec53d7ec45554aa80f"`


#### Quick Links

[Back](client.md) [Home](../readme.md)

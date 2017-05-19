Debt Panel Introducer API
=========================
Debt Panel Introducer API

**Version:** 1.0.0

**Contact information:**  
ss@beyondcomparison.com  











### /clients/{reference}/status
---
##### ***PATCH***
**Summary:** update the status of the client

**Description:** Updates a Client to show the current status

**Parameters**

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| reference | path | The reference given on transferring the lead | Yes | string |
| body | body | Details of the status being updated | No | [StatusUpdate](#statusUpdate) |

**Responses**

| Code | Description | Schema |
| ---- | ----------- | ------ |
| 200 | Update was successful | [Basic200](#basic200) |
| 404 | Client reference number was not found | [Error404](#error404) |

**Security**

| Security Schema | Scopes |
| --- | --- |
| ExternalApiKeyHeaderParam | |

### /clients/{reference}/notes
---
##### ***POST***
**Summary:** adds a note to the client

**Description:** Attaches a note to the client

**Parameters**

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| reference | path | The reference given on transferring the lead | Yes | string |
| body | body | Details of the note being added | No | [AttachNote](#attachNote) |

**Responses**

| Code | Description | Schema |
| ---- | ----------- | ------ |
| 200 | Addition was successful | [Basic200](#basic200) |
| 404 | Client reference number was not found | [Error404](#error404) |

**Security**

| Security Schema | Scopes |
| --- | --- |
| ExternalApiKeyHeaderParam | |

### Models
---
<a name="submission"></a>**Submission**  


<a name="leadResponse"></a>**LeadResponse**  

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| success | boolean |  | No |
| message | string |  | No |
| data | [LeadId](#leadId) |  | No |
<a name="leadId"></a>**LeadId**  

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| leadId | string |  | No |
<a name="lead"></a>**Lead**  


<a name="address"></a>**Address**  


<a name="contactDetails"></a>**ContactDetails**  


<a name="statusUpdate"></a>**StatusUpdate**  

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| status | string |  | Yes |
| note | string |  | No |
<a name="attachNote"></a>**AttachNote**  

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| note | string |  | Yes |
<a name="error400"></a>**Error400**  

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| success | boolean |  | No |
| message | string |  | No |
<a name="error401"></a>**Error401**  

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| success | boolean |  | No |
| message | string |  | No |
<a name="error403"></a>**Error403**  

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| success | boolean |  | No |
| message | string |  | No |
<a name="error404"></a>**Error404**  

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| success | boolean |  | No |
| message | string |  | No |
<a name="error409"></a>**Error409**  

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| success | boolean |  | No |
| message | string |  | No |
<a name="basic200"></a>**Basic200**  

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| success | boolean |  | No |
| message | string |  | No |
<a name="apiStatus"></a>**ApiStatus**  

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| success | boolean |  | No |
| message | string |  | No |
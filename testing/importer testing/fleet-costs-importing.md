![[costimport.xlsx]]### Fleet costs importing:

This page serves as a guide for testing the importer functionality related to cost importing. The testing process is dated [[#Date]] and revolves around evaluating the effectiveness and accuracy of the cost importing feature. The page is organized into several sections for easy navigation.

### Date:

28/07/2023

### Tags:

[[importer]] 

### Summary:

This testing will cover the importer test for costs.

### Table of Contents:

- [[#Notes]]
- [[#Related Notes]]
- [[#References]]
- [[#Backlinks]]
- [[#Attachments]]

### Notes

When importing the costs for cost import you'll need to first start with the file. I've attached the test files bellow [[#Attachments]].  

	We need:
	- Reg
	- Vin
	- Company code
	- Group code
	- Supplier code

- If the supplier isn't found it'll create a new one.
- Multilease suppliers
- Cost group code
- Group has to be part of the company
- Only need to specify the company. The rest will be read from the spreadsheet.

<details>
<summary>Transaction fields to import</summary>
<ul>
<li>Mapping name</li> 
<li>Unique key</li> 
<li>Gross</li>
<li>Net</li>  
<li>Vat</li>  
<li>Vat rate</li>  
<li>Total</li>  
<li>Client number</li> 
<li>Client country</li> 
<li>Invoice number</li> 
<li>Vrn</li> 
<li>Vin</li> 
<li>Invoice date</li> 
<li>Invoice line code</li> 
<li>Invoice line description</li> 
<li>Group code</li> 
<li>Cost group code</li> 
<li>Provider Company</li>  
<li>mapping</li> 
<li>company = select on the next page</li> 
<li>cost Group = cost group code</li> 
<li>group = group code</li> 
<li>vehicle = vrn</li> 
<li>supplier = provider</li> 
<li>currency = select on next page</li> 
</ul>
</details>


<details>
<summary>Match transaction fields with unique identifiers</summary>
<ul>
<li>select transaction primary key or unique key field = transaction reference</li>
<li>select on provider company mapping item = default-provider</li>
<li>Select one company item = "Select the company"</li>
<li>Select costGroup = code</li>
<li>Select group = GroupCode</li>
<li>Select vehicle = licenseplatenumber</li>
<li>Select costGroup = code</li>
<li>Select supplier = code</li>
<li>Select one currency item = GBP</li>
</ul>
</details>

- transaction reference
- Select company.
- Match field with fields in database
- Find something with code or "name" - code 
- vehicle always maps to licence plate number
- supplier = name

After the import you'll need to run the job on [[aws-terminal-tutorial]]
#### Areas to cover:

```mermaid
flowchart TD
A[Take file] --> B[Check file] --> C[Run through import] --> D[Compare file with transactions] --> E[Compare file with transaction links]
```


### Related Notes:

none.

### References:

[[staging]](https://staging.ultraportal.co.uk/secure/dashboard)

### Backlinks:

none

### Attachments:

![[costimport.xlsx]]

working mapping:

```
{"primaryKey":"row_content_uid","fields":{"gross":"gross","net":"Net","vat":"vatcode","vatRate":"vatrate","total":"Net","clientNo":"Clientname","clientCountry":"Clientcountry","supplierName":"Provider","invoiceNumber":"Invoicenumber","vrn":"VRN","vin":"VIN","invoiceDate":"Invoicedate","invoiceLineCode":"Invoicelinecode","invoiceLineDescription":"Invoicelinedescription","invoiceLineAdditionalDescription":"Invoicelineadditionaldescription","groupCode":"groupcode","costGroupCode":"costgroupcode","providerCompanyMapping":"select_later"},"associations":{"providerCompanyMapping":{"isNullable":false,"className":"App\\Entity\\Core\\Cost\\ProviderCompanyMapping","uniqueField":"ID","value":"1"}},"dateFields":["snapshotDate","dateCreated","dateUpdated","invoiceDate","localeTime","utcTime"],"providerFields":{"company":"select_later","costGroup":"costgroupcode","group":"groupcode","vehicle":"VRN","supplier":"Provider","currency":"select_later"},"providerAssociations":{"company":{"isNullable":true,"className":"App\\Entity\\Classic\\Company","uniqueField":"ID","value":"1255810"},"costGroup":{"isNullable":true,"className":"App\\Entity\\Core\\Cost\\Group","uniqueField":"code"},"group":{"isNullable":true,"className":"App\\Entity\\Classic\\Group","uniqueField":"GroupCode"},"vehicle":{"isNullable":true,"className":"App\\Entity\\Classic\\Vehicle","uniqueField":"licenseplatenumber"},"supplier":{"isNullable":true,"className":"App\\Entity\\Core\\Cost\\Supplier","uniqueField":"name"},"currency":{"isNullable":true,"className":"App\\Entity\\Core\\Enum\\Currency","uniqueField":"ID","value":"5"}},"uniqueField":"transactionReference","actions":{"default":["PROCESS_TIME_ZONE","MATCH_SUPPLIER","SET_COST_GROUP","SET_CURRENCY_CODE"]},"configurations":{"default":{"PROCESS_TIME_ZONE":{"utcOffset":"+0100","dayLightSaving":true,"timezone":"Europe\/London","utcTime":"2023-07-28 13:19:22","localeTime":"2023-07-28 14:19:22"},"SET_CURRENCY_CODE":{"currency":"GBP"}}}}
```

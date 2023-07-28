### Inventory importing:

This page serves as a guide for testing the importer functionality related to inventory importing. The testing process is dated [[#Date]] and revolves around evaluating the effectiveness and accuracy of the cost importing feature. The page is organized into several sections for easy navigation.

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

body style = type 
Company = select company
group = group code
vehicle = licenceplate 
number = name
currency code = code

#### Areas to cover:

```text
compare file with inventory item

compare file with the inventory mapping

Make sure funding type is set

check entity mapping

Go to vehicle and check data is correct
```

### Related Notes:

none.

### References:

[staging ultraportal](https://staging.ultraportal.co.uk/secure/dashboard)

### Backlinks:

none

### Attachments:

![[uk_roi_test_file.csv]]
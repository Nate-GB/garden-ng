---
title: "Data Types"
tags:
- sapling
- data
- security
---

A data type schema usually applies more detailed labels than [Data Classification](notes/Data%20Classifications.md).

- [Personally Identifiable Information](notes/Personally%20Identifiable%20Information.md) 
	- Data can be used to identify, contact, or locate and individual
	- Several types of PII, including:
		- SSN
		- name
		- date of birth
		- email address
		- telephone number
		- street address
		- biometric data
	- Some information could be PII depending on context. A static IP address could be PII when browsing the web, for example
	- Often used for password reset mechanisms and over-the-phone identification, like with security questions
- [[Customer Data]]
	- Can be institutional information, but also [Personally Identifiable Information](notes/Personally%20Identifiable%20Information.md)
		- Customer's employees
		- Sales
		- Tech support contacts
	- PII for customers basically
	- Could be shared under a [NDA](notes/NDA.md)
- [[Financial Information]]
	- [[PCI DSS]] defines the safe handling and storage of financial information
	- This is data involving money, like bank and investment accounts, payroll, and tax returns
- [Personal Health Information](Personal%20Health%20Information)
	- PHI
	- medical and insurance records, plus hospital and lab test results
	- Could be associated with a specific person, but also could be anonymized
	- Very valuable on black market, used for insurance fraud or victim blackmail
	- *Extremely* [Sensitive Data](Sensitive%20Data.md)
- [[Government Data]]
	- Internal government agency data
	- requirements placed by federal law in the US

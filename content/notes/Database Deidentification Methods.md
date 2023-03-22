---
title: "Database Deidentification Methods"
tags:
- sapling
- data
- security
---

Deidentification methods are usually implemented as part of the database management system hosting the data. [Sensitive](notes/Sensitive%20Data.md) fields will be tagged for deidentification whenever a query or report is run.

# Types of Deidentification

- [[Data Masking]]
	- A field might be partially redacted to preserve metadata for analysis purposes
	- Irreversible
- [[Tokenization]] 
	- All or part of date in a field is replaced with a randomly generated token
	- Original value can be retrieved if necessary by authorized party
	- Substitute for encryption
- [[Aggregation or Banding]]
	- Generalizes the data, such as substituting a specific age with a broader age range
- [[Hashing and Salting]]
	- Used for either indexing or storage for data that shouldn't be plaintext

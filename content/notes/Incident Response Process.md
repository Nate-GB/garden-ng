---
title: "Incident Response Process"
tags:
- sapling
- security
---

Defined by [NIST 800.61r2](https://wmx-api-production.s3.amazonaws.com/courses/5721/supplementary/NIST.SP.800-61r2.pdf), incident response follows a well-structure process.  There are 6 principal stages in an incident response lifecycle.

1. Preparation
	1. Make the system resilient to attack in the first place. This includes hardening systems, writing policies and procedures, and setting up confidential lines of communication. It also implies creating incident response resources and procedures
2. Identification
	1. From the information in an alert or report, determine whether and incident has taken place, assess how sever it might be, and notify stakeholders
3. Containment
	1. Limit the scope and magnitude of the incident. The goal of incident response is to secure data while limiting the immediate impact on customers and business partners
4. Eradication
	1. Remove the cause and restore the affected system to a secure state by wiping a system and applying secure config settings
5. Recovery
	1. The system can now be reintegrated.  Applying patches and updates toa  system to help prevent future incidents is important as well. This phase may involve restoration of data from backup and security testing.  Systems must be monitored more closely for a period to detect and prevent any reoccurrence of the attack. The response process may gave to iterate through multiple phases of identification, containment, eradication, and recovery to effect a complete resolution.
6. Lessons Learned
	1. Analyze the incident and responses to identify whether procedures or systems could be improved. It is imperative to document the incident. The outputs from this phase feed back into a new preparation phase in the cycle.


![Incident Response Lifecycle](notes/images/Incident%20Repsonse%20Lifecycle.jpg)
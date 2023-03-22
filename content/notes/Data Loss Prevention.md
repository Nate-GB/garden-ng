---
title: "Data Loss Prevention"
tags:
- sapling
- data
- security
---

# Keep that data safe

- Usually an automated tool
- Can protect [[Intellectual Property]] data
- Will usually consist of three components
	- Policy Server to configure classification, confidentiality, and privacy rules and polices, log incidents, and compile reports
	- Endpoint Agents to enforce policy on client computers, even when they are not connected to the network
	- Network Agents to scan communications at network borders and interface with web and messaging servers to enforce policy
- DLP agents scan content in structured formats, like databases with a formal access control model
- DLP agents can also scan content in unstructured formats, like emails or word processing documents
- DLP agents can block the transfer of content if it does not conform to a predefined policy
	- (Side note, this is probably what the Pope-blessed laptop used)

# Remediation

- The action a DLP software takes when it detects policy violation
	- Alert only
	- Block
	- Quarantine
	- Tombstone
		- The file is quarantined and replaced with one describing the policy violation and how the user can release it again

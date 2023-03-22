---
title: "Cyber Kill Chain"
tags:
- seed
- security
---

A framework that describes the stages of a cyber attack

1. Reconnaissance
	1. Scoping out the target
2. Weaponization
	1. Preparation of attack based on recon from previous step
	2. Could be payload code + exploit code
3. Delivery
	1. Weaponized code is transmitted to target system
4. Exploitation
	1. Weaponized code is executed on the system
5. Installation
	1. Weaponized code runs a remote access tool (RAT) and achieves persistence on target system
6. Command and control
	1. Outbound channel is established to remote server that allows the attacker to control the RAT 
7. Actions on objectives
	1. Access is used to collect information and exfiltrate information from target
	2. There could be other goals or motives

![Cyber Kill Chain](notes/images/cyber-kill-chain.jpg)

See Also: [[MITRE ATT&CK]] and [[Diamond Model]] 
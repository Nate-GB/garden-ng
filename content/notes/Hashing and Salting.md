---
title: "Hashing and Salting"
tags:
- seed
- data
- security
---

A method of producing a fixed-length string from arbitrary-length plaintext data using an algorithm, like SHA.  It should be impossible to match the hash back to a plaintext.  Often used to prove integrity.

Salting is the process of storing an additional value to the plaintext before hashing. This is meant to make cracking the hash more difficult for a malicious actor.  

See also: [CIA Triad](notes/CIA%20Triad.md)

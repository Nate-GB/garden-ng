---
title: "Backups"
tags:
- sapling
- data
- security
---

The practice of creating and storing copies of data in order to allow data restoration in the event of a failure or loss of the original data.

There are 3 main types of backups:
- [[Full Backups]]
- [[Incremental Backups]]
- [[Differential Backups]]

A large downside to backups as a primary means of recovery is the issue of "open files." For systems such as databases or Exchange messaging systems, file backups will often leave out open files as they are continually being edited. This can leave a large gap in your recovery methods. However, there is a way around this. Enter,

# Snapshots

Snapshots are similar to backups, but rather than focusing on files they essentially take a "picture" of an file system.  Backup programs are then able to restore from these snapshots. A snapshot is a point-in-time copy of data maintained by the file system. Snapshots are provided by the Volume Shadow Copy Service on NTFS volumes. 

Snapshots can also be made of [[Virtual Machines]].

# Images

Images are like snapshots, but for entire systems. An image backup duplicates an OS installation. It's like flash-freezing a cave man; once you thaw him out, it's like no time has passed at all.  


# Backup Storage

Backups need to be stored as securely as live data, so it's essentially the same data tucked away for emergencies.  If the origin data is highly confidential and has a high integrity requirement, then so must the backup data.  Availability is a little bit different, but is still something that must be carefully considered.  

To prepare for large-scale events that could threaten both the live data and the backup, it's usually good practice to keep some of your backups offsite.  This can enable a faster recovery time in the event of a natural disaster, for example. However, you must ensure you are either able to support the bandwidth needed to transmit the data or a reliable way to move physical copies to your offsite storage for it to be an effective method of storage. 

You also need to consider online storage vs offline storage.  To do so, you need to evaluate the balance between availability and security that is acceptable to you. This will obviously differ for each company and even each person, so find the balance that's right for your purposes. Offline storage is not as easily accessible in the event of an emergency, but it is considerably more secure. Online storage is almost immediately accessible, but at the cost of increased risk of security incidents. 

A general rule of thumb that's widely accepted in backup storage is called the [[3-2-1 Rule]]. 

# Backup Media Types

There are several different types of media available to store your backups on. Here's a few:

- Disk
	- Removeable hard drives
	- Low Cost option
	- Not a large enough capacity for enterprise backup solutions
- Network Attached Storage
	- Usually utilizes a RAID storage protocol
	- Available over common network protocols
	- File-level backups
	- No offsite option
- Tape
	- Very cost effective
	- Easily transported offsite
	- High storage capability
	- Slow compared to disk-based solutions
- Storage Area Network (SAN) and Cloud
	- Block-level addressing
	- can use multiple RAID arrays
	- Can achieve offsite storage through replication


# Restoration

In the event of an outage or incident, there is a specific order that services and systems should be brought back online and verified.  This is referred to as the [[Order of Restoration]]. If systems are brought back online in an uncontrolled way, there is serious risk of causing additional power problems or of causing problems in the network, OS, or application layers due to dependencies between these. 
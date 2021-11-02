# CIT 114 Week 9
## Here are some important thinkgs I learned in Week 9
### Notes 07: Storage

#### What is Storage?

Before you can choose what type of storage you should use with a cloud computing provider, you first need to understand what is storage. Storage is basically a technology that allows a user to retain digital data onto a medium. It is one of the core components of a computer and in cloud computing, something that you need to understand the differences.

In a computer, there are two types of storage: Volatile and Non-Volatile.

Volatile memory - is a type of storage whose contents are erased when the system's power is turned off or interrupted. For example, RAM is volatile. When you are working on a document, it is kept in RAM, and if the computer loses power, your work will be lost. For this reason, you should save your document to a file on a non-volatile storage medium, such as your hard drive.

NV or Non-volatile - memory is a term used to describe any memory or storage that is saved regardless of the power to the computer is on or off. It is also called persistent storage or permanent storage. An example of non-volatile memory and storage is a computer hard drive, flash memory, and ROM. If data is stored on a hard drive, it will remain on that drive regardless if the power is interrupted, which is why it is the best place to store your data and documents. Non-volatile memory also stores your computer's time and system settings even when the power is off.

Local Storage Types

In computing, there is many forms of storage. Temporary storage, such as RAM, allows a computer to temporarily store information while the computer is in use, however when power is removed, the information stored in temporary storage is lost. Permanent storage is where you keep your operating system, applications, and other data files that you use on a computer system. The information will be saved even if there is no power to the system.

------

Read Only Memory (RAM)

As the computer boots, parts of the operating system and drivers are loaded into memory (RAM), which allows the CPU to process the instructions faster and speeds up the boot process. RAM is temporary storage that allows data and programs to be stored in memory in order the operating system to use them. After the operating system has booted up, each program you open, such as the browser you're using to view this page, is loaded into memory while it is running. If too many programs are open, the computer will swap the data in the memory between the RAM and the hard disk drive.

A computer's performance is largely attributed to the amount of memory contained within it. If a computer does not have the recommended memory to run the operating system and software programs being used, it will result in slower performance. The more memory a computer has, the more information and software it can load and process quickly.

------

Hard Drives

A hard drive can be used to store any data, including pictures, music, videos, text documents, and any files created or downloaded. Also, hard drives store files for the operating system and software programs that run on the computer. The two main types of hard drive are HDD (hard disk drive) and SSD (solid state drive).

|Topic|SSD|HDD|
|---|---|---|
|Access time|An SSD has access speeds of 35 to 100 microseconds.|A typical HDD takes about 5,000 to 10,000 microseconds to access data.|
|Price|The price of a solid-state drive is higher than an HDD, which is why most computers with an SSD only have a few hundred gigabytes of storage.|HDD is considerably cheaper than SSD, especially for drives over 1 TB.|
|Reliability|The SSD has no moving parts. It uses flash memory to store data, which provides better performance and reliability over an HDD.|The HDD has moving parts and magnetic platters, meaning the more use they get, the faster they wear down and fail.|
|Capacity|Although there are large SSDs, anything over 1 TB SSD is usually outside of most people's price range.|Several terabyte hard disk drives are available for very reasonable prices.|
|Power|The SSD uses less power than a standard HDD, which means a lower energy bill over time and for laptops, an increase in battery life.|With all of the parts required to spin the platters, the HDD uses more power than an SSD.|
|Noise|With no moving parts, SSD generates no noise.|With the spinning platters and moving read/write heads, an HDD can sometimes be one of the loudest components in your computer.|
|Heat|Because there are no moving parts and due to the nature of flash memory, the SSD generates less heat, helping to increase its lifespan and reliability.|With moving parts comes added heat which can slowly damage electronics over time, so the higher the heat, the greater the potential for wear and damage.|
|Magnetism|SSD is not affected by magnetism.|Because a hard drive relies on magnetism to write information to the platter, the information could be erased from an HDD using strong magnets.|

------

Optical Drive

Another common storage is optical storage, which uses lasers and lights as its method of reading and writing data. The three standards of optical media are CD (compact disk), DVD (digital versatile disk or digital video disk), and Blu-ray. All standards use the same size disc, but the data is read differently for each. Below is a table of data capacity for each standard.

|CD|DVD|Blu-ray|
|---|---|---|
|700 MB|Single-sided, single-layer: 4.7 GB Single-sided, double-layer: 8.5-8.7 GB Double-sided, single-layer: 9.4 GB Double-sided, double-layer: 17.08 GB|Single-layer disc: 25 GB Dual-layer disc: 50 GB|

------

Flash Drive

Referred to as a USB flash drive, data stick, pen drive, memory unit, keychain drive, and thumb drive, a jump drive is a portable storage device. It is often the size of a human thumb (hence the name) and connects to a computer via a USB port. Flash drives are an easy way to store and transfer information between computers and range in sizes from 2 GB to 1 TB.

Unlike a standard hard drive, the flash drive has no movable parts; it contains only an integrated circuit memory chip that is used to store data. Flash drives usually have plastic or aluminum casings surrounding the memory chip.

------

#### Disaster Recovery and Technology

Should the unthinkable happen, how do you recover? A disaster is anything that puts a business at risk from a natural disaster, equipment failure or cyberattack. Simply put, disaster recovery is a set of policies, tools, and procedures that enable the recovery or continuation of critical IT infrastructure and systems following a disaster. Storage is one of those key areas you want to carefully plan your recovery.

Disaster recovery (DR) starts with a plan that works in conjunction with the business continuity and contingency plans. In DR, the goal is to get a business back operating as normally as possible as quickly as possible. This involves a lot of planning, skill at troubleshooting, and practice of the DR plan that may involve full drills practicing the written steps then updating them with changes.

However, the first step in recovering from a disaster is making sure that the disaster is over. You cannot start the recovery until the fire is out and IT personal are in position to start the recovery.

------

Fault Tolerance

What if you have a server at a business and the hard drive fails? If you have a single hard drive, then your system is down until you can replace it. Fault tolerance is the idea that a system can continue to run properly even in the event of a failure of a component of that system. The ability to tolerate a failure of a critical component in a system and maintain functionality is also referred to as graceful degradation.

When you design a system that will tolerate failures, the system will continue to work as expected rather than work at a reduced level or fail entirely. To do this you need to reduce the single points of failure like having a single hard drive act as a backup, isolate failures or contain failures and be able to reverse issues. This is where replication, redundancy and backups create a fault tolerant system.

Replication and redundancy sound similar but that have different meanings in the IT world, especially when it comes to being fault tolerant.

------

Replication

Replication of IT infrastructure and data means that you have a full working duplicate of the data, systems, and networks that are critical. Replicated systems may be used at the same time to provide distribution of workloads across multiple identical systems. In terms of data, replicated data is written to multiple hard drives possibly in multiple locations.

Replication is the most expensive of the fault tolerant options, in traditional infrastructure, as it requires to you to have multiple identical systems in place for each area you want to replicate. In large businesses, replicated data centers are called hot sites, as they have everything required to get a business back up in running including power, data and networking.

------

Redundancy

Redundancy is the idea where you have IT infrastructure in place to keep a business running, but it may be at a reduced capacity. The infrastructure may not be identical nor powerful enough to run on for a long period of time, but it will be good enough to run a business while the problem that caused the failure is identified and fixed.

Replicating data takes planning and redundant equipment. You can easily manually copy important information to a different hard drive, USB drive, or cloud storage, but will you always remember to do that every time you save a document.

------

#### Storage in the Enterprise

As an individual, a single hard drive is sufficient for a computer to run your operating system and save your files. However, in large or complex businesses this will not suffice.
An enterprise is generally a large business that has hundreds if not thousands of employees. These types of businesses require IT solutions that are both knowledge-intensive and require significant investment. However, the tools that enterprise IT uses can be used by anyone willing to put the time, money, and effort into setting one up.

------

Redundant Array of Independent Disks (RAID)

The simplest way to replicate data is to use a Redundant Array of Independent Disks or RAID for short. Depending on the level you use, you can lose a drive and still keep all your data safe. Computers and servers can use a RAID to replicate data across multiple redundant drives in order to ensure data is available.

RAIDs are used often as part of other devices such as Network Attached Storage, Storage Area Networks, as well as internal drives for a Computer or File Server.

The most common levels used by businesses for backups are RAID 1, RAID 5, RAID 6 and RAID 1+0.

|RAID Level|Description|
|---|---|
|RAID 0|Disk stripping. Data is written across two or more drives. This does not create any redundancy but does increase read speed.|
|RAID 1|Disk mirroring. Data is written identically to two drives creating a mirrored set. Slowest write speed of all the RAID as all data must be written to all drives.|
|RAID 5|Block-level stripping with a distributed parity. Requires a minimum of three drives and can operate with a single drive failure.|
|RAID 6|An extension of RAID 5 with an additional parity block. Requires a minimum of four drives and can operate with two disk failures.|
|RAID 1+0|A hybrid RAID that involves having two stripped sets of disks then mirroring them. Provides the best benchmarks for intensive systems like databases, web and email servers as it|

------

File Servers

In a technical sense, a server is an instance of a computer or device that accepts and responds to requests made by another program, known as a client. A good metaphor would be a customer (client) ordering a package then the mailman (server) delivering it to them or someone else.

A file server is a type of server on a network that is used to provide authorized users with access to files. It has all of the same components that a computer or server has including a CPU, RAM and storage, but the storage used for serving files is generally larger and optimized for serving files. Normally file servers are kept off of the public internet for security reasons, but are available on an internal enterprise network.

------

Network Attached Storage (NAS)

NAS is short for Network Attached Storage. A NAS device is any storage device that is connected to a network and provides a network with additional storage. A NAS does not have any processing power on its own, meaning it cannot be used to execute or run network shared programs. Most home routers today have a USB port allowing for an external hard drive to be connected as a NAS. In this configuration, anyone connected to the router can access the hard drive.

A NAS will present and manage file systems for any client computers who are authorized to access it over the Internet.

------

Storage Area Network (SAN)

A Storage Area Network, SAN for short, is a specialized high-speed network that provides access at a raw block-address level. Systems can attach it to servers using technologies like Fiber Channel (FC) or Internet Small Computing System Interface (iSCSI) so that the storage appears to be attached locally rather than connected via a network.

A SAN will provide other compuers with raw block-address level storage capacity by attaching it to those systems.

------

#### Storage in the Cloud

Cloud storage is a cloud computing model that stores data on the Internet through a cloud computing provider who manages and operates data storage as a service. It’s delivered on demand with just-in-time capacity and costs, and eliminates buying and managing your own data storage infrastructure. This gives you agility, global scale and durability, with “anytime, anywhere” data access.

Cloud storage uses many of the same technologies as Enterprise IT storage solutions, but at a significantly larger scale. As a consumer of Cloud Storage, you do not have any visibility to how they are setup, but will know how to utilize them.

All of those services listed utilize cloud storage to enable your ability to access files from anywhere you have internet.

You may already be familiar with cloud storage if you have used:
  * Google Drive
  * Dropbox
  * Box.com
  * Microsoft Onedrive
  * And more...

------

How Does Cloud Storage Work?

Cloud storage is purchased from a third party cloud vendor who owns and operates data storage capacity and delivers it over the Internet in a pay-as-you-go model. These cloud storage vendors manage capacity, security and durability to make data accessible to your applications all around the world.

Applications access cloud storage through traditional storage protocols or directly via an API. Many vendors offer complementary services designed to help collect, manage, secure and analyze data at massive scale.

------

Benefits of Cloud Storage


Storing data in the cloud lets IT departments transform three areas:

Total Cost of Ownership

With cloud storage, there is no hardware to purchase, storage to provision, or capital being used for "someday" scenarios. You can add or remove capacity on demand, quickly change performance and retention characteristics, and only pay for storage that you actually use. Less frequently accessed data can even be automatically moved to lower cost tiers in accordance with audit-able rules, driving economies of scale.

Time to Deployment

When development teams are ready to execute, infrastructure should never slow them down. Cloud storage allows IT to quickly deliver the exact amount of storage needed, right when it's needed. This allows IT to focus on solving complex application problems instead of having to manage storage systems.

Information Management

Centralizing storage in the cloud creates a tremendous leverage point for new use cases. By using cloud storage lifecycle management policies, you can perform powerful information management tasks including automated tiering or locking down data in support of compliance requirements.

------

Cloud Storage Requirements

Ensuring a company's critical data is safe, secure, and available when needed is essential. There are several fundamental requirements when considering storing data in the cloud.

   * Durability: Data should be redundantly stored, ideally across multiple facilities and multiple devices in each facility. Natural disasters, human error, or mechanical faults should not result in data loss.
   * Availability: All data should be available when needed, but there is a difference between production data and archives. The ideal cloud storage will deliver the right balance of retrieval times and cost.
   * Security: All data is ideally encrypted, both at rest and in transit. Permissions and access controls should work just as well in the cloud as they do for on premises storage.

------

Types of Cloud Storage

There are three types of cloud data storage: object storage, file storage, and block storage. Each offers their own advantages and have their own use cases:

1.	Object Storage (Links to an external site.) - Applications developed in the cloud often take advantage of object storage's vast scalability and metadata characteristics. Object storage solutions are ideal for building modern applications from scratch that require scale and flexibility, and can also be used to import existing data stores for analytics, backup, or archive.
2.	File Storage (Links to an external site.) - Some applications need to access shared files and require a file system. This type of storage is often supported with a Network Attached Storage (NAS) server. File storage (Links to an external site.) solutions are ideal for use cases like large content repositories, development environments, media stores, or user home directories.
3.	Block Storage - Other enterprise applications like databases or ERP systems often require dedicated, low latency storage for each host. This is analagous to direct-attached storage (DAS) or a Storage Area Network (SAN). Block-based cloud storage solutions are provisioned with each virtual server and offer the ultra low latency required for high performance workloads.

------

#### Five Ways to Use Cloud Storage

Backup and Recovery

Backup and recovery is a critical part of ensuring data is protected and accessible, but keeping up with increasing capacity requirements can be a constant challenge. Cloud storage brings low cost, high durability, and extreme scale to backup and recovery solutions. Embedded data management policies like Amazon S3 Object Lifecycle Management can automatically migrate data to lower-cost tiers based on frequency or timing settings, and archival vaults can be created to help comply with legal or regulatory requirements. These benefits allow for tremendous scale possibilities within industries such as financial services, healthcare, and media that produce high volumes of data with long-term retention needs.

Software Test and Development

Software test and development environments often requires separate, independent, and duplicate storage environments to be built out, managed, and decommissioned. In addition to the time required, the up-front capital costs required can be extensive.

Some of the largest and most valuable companies in the world have created applications in record time by leveraging the flexibility, performance, and low cost of cloud storage. Even the simplest static websites can be improved for an amazingly low cost. Developers all over the world are turning to pay-as-you go storage options that remove management and scale headaches.

Cloud Data Migration

The availability, durability, and cost benefits of cloud storage can be very compelling to business owners, but traditional IT functional owners like storage, backup, networking, security, and compliance administrators may have concerns around the realities of transferring large amounts of data to the cloud. Cloud data migration services services such as AWS Import/Export Snowball can simplify migrating storage into the cloud by addressing high network costs, long transfer times, and security concerns.

Compliance

Storing data in the cloud can raise concerns about regulation and compliance, especially if this data is already stored in compliant storage systems. Cloud data compliance controls like Amazon Glacier Vault Lock are designed to ensure that you can easily deploy and enforce compliance controls on individual data vaults via a lockable policy. You can specify controls such as Write Once Read Many (WORM) to lock the data from future edits. Using audit log products like AWS CloudTrail can help you ensure compliance and governance objectives for your cloud-based storage and archival systems are being met.

Big Data and Data Lakes

Traditional on-premises storage solutions can be inconsistent in their cost, performance, and scalability — especially over time. Big data projects demand large-scale, affordable, highly available, and secure storage pools that are commonly referred to as data lakes.

Data lakes built on object storage keep information in its native form, and include rich metadata that allows selective extraction and use for analysis. Cloud-based data lakes can sit at the center of all kinds data warehousing, processing, big data and analytical engines, such as Amazon Redshift, Amazon RDS, Amazon EMR and Amazon DynamoDB to help you accomplish your next project in less time with more relevance.

------

#### Encrypting Storage

One of the things IT professionals must think about is how can we protect data from being compromised both at rest and in transit. Encryption is a method securing data by taking data and making it unreadable without the right decryption information.

To understand encryption, you must first understand that there are two types of text:
  * Plain text is the original message or information before it has been encrypted. This text can be read by anyone as it is readable text.
  * Cipher text is the encrypted version of the original plain text message after algorithm called a cipher has been applied to it. The encryption algorithm takes the plain text message and makes it so that it is no longer readable text.

The Caesar Cipher is one of the most historically well-known ciphers this is known as a substitution cipher where one letter is substituted for another. In the case below, this is using a left shift of three characters where you take the original letter and shift it three letters to the left so, T becomes Q, H becomes E, E becomes B, and so on.

Plaintext:  THE QUICK BROWN FOX JUMPS OVER THE LAZY DOG

Ciphertext: QEB NRFZH YOLTK CLU GRJMP LSBO QEB IXWV ALD

This can easily be symmetrically decrypted, using pen and paper, by shifting each letter back three letters to the right. So, this classical cryptography method will not work for modern encryption to keep your information safe.

That is where public-key cryptography or asymmetric cryptography comes into play. In public-key cryptography, two paired keys are used encrypt and decrypt messages. The public-key can be given to anyone for the purpose of encryption. The private-key is known only to the owner of the keys and is used for decryption.

------

Data at Rest

Data at rest simply means that the information is being stored physically where it is inactive or in use but not in being actively transmitted over a network. This data is most at risk for being stolen via physical theft or unauthorized access to file storage.

There are several ways to protect data at rest through file or disk level encryption in order to protect the information being stored on the device from theft or unauthorized access.

Encryption on most modern operating systems can be done one of two ways, at the file level or disk level. The difference between the two is that in the file level, you choose which files are encrypted and which are not, while the disk level encrypts everything including the operating system.

File level encryption allows you to specific files or folders on a device to encrypt. This can be done manually or automatically depending on the encryption software and will render the files unreadable without the decryption software and key.

------

Data in Transit

Data encryption while files are in transit is different that encryption at rest. When a file is in transit, you have two or more computers involved. The sender is the original system who encrypts the information being sent while the receiver are the systems that decrypt the information upon receipt.
  * Email is one of the most common forms of communication for businesses and was originally not designed to encrypt messages. Various forms of encryption were added over the years such as STARTTLS, a common transport-level encryption protocol, or S/MIME which allows for enhanced encryption. All major email providers and email servers support encryption, but it is important to know that the sender and receiver must both support the same level of encryption in order for a message to be read. Want to know how Gmail encrypts your email, find out about how you can determine if an email is being encrypted before it is sent.
  * HTTPS, is probably the encryption technology you are most familiar with and by now you know to look for the https:// or the browser lock symbol in the browser address bar. HTTPS is the secure version of the HTTP protocol, so any information like logins or credit cards will be encrypted during the transmission.
  * VPN stands for Virtual Private Network and it will create a secure connection between two systems extending a private network to a remote user. This is most often used by businesses where they need a secure connection between a remote employee and the private business network. All traffic between the two locations is authenticated and encrypted.
  * Mobile applications are trickier to know if they are encrypting data in transit. In general, the same standards for Windows and Mac desktop computers can also apply to mobile devices for encrypting data at rest and in transit. Apple has entire documentation regarding how applications should handle data encryption in transit, however that does not mean it will be used incorrectly.

------

#### Data Backups

Having redundant drives in a RAID is a good start to having your data backed up, however it is not a true backup strategy. Data can be lost, damaged, compromised, or stolen due to user error, equipment failure, malware or hacking.

The data and information you can generate from it is valuable asset. Loss of data due to any of these can cause significant disruption in a business.

Types of Backups:

Backup software works by looking for an attribute of a file called the archive bit. When a file is created or modified, the archive bit is set to 1 indicating to the backup software that it needs to be backed up. Once a backup is made, the archive bit is reset to 0 indicating that the backup software has archived the file and cleared the flag. Depending on the software, it may or may not clear the archive bit.

  * Full or Normal: Backs up every selected files or folders in full then clears the archival bit. This backup takes the longest and most space but is faster to restore.
  * Copy: Makes a copy and backups up selected files or folders regardless of modification date or archive bit status. Does not clear the archive bit.
  * Incremental: After completing a full backup, it backs up changes made to selected files that modified since the last backup then clears the archival bit.
  * Differential: After completing a full backup, it backs up changes made to selected files that were modified since the last full backup and does not clear the archival bit.
  * Daily: Backs up files that were created or modified today. It ignores the archive bit, looking at the modification date only. 

------

#### Backup Locations

Disasters happen. Maybe you have warning, maybe you do not. What would happen if all you had was backups inside your business location and the unimaginable happened, a fire burned down your business (there is a real story about this at the end of the section).

The location of your backups should be kept into consideration as a part of your business continuity plan. Your backup strategy should include both local backups (on-site) as well as cloud or remote backups (off-site).

------

Stored Locally

Backups that are stored locally generally use an external hard drive, RAID, network attached storage (NAS), USB drive or even a DVD, where the backup is in the same physical location (on-site) as the business.

Backups stored locally will be faster to backup and restore. The shorter data transfer distance will decrease the amount of time it takes to restore files and get a business back up and running. However, they are at greater risk if the entire business is destroyed including all the backups. A flood or power surge can easily destroy all electronics if not properly protected leaving you with no backups.

------

Cloud Storage

Cloud storage allows for a business to move the backup to cloud storage infrastructure outside of the business location. Saving important data to cloud storage such as Google Drive, Dropbox, or Box.com can help move data outside away from the local business. This is great for easy always on access where you can modify files directly in those solutions. However, companies like Amazon, Google and Microsoft have also have storage solutions available to put critical backups

There is also now an entire class of backup software, where for a subscription, your data is transmitted over the internet and stored remotely in the cloud. This software is typically very easy to setup and use. It also has built in security to ensure your data is encrypted prior to leaving your computer for the cloud. This will prevent hackers from being able to easily recover or restore your remote data.

Companies like CrashPlan, Backblaze, and Carbonite are some of the leading business and consumer cloud backup services.

------

On-site vs Off-site

An on-site backup is the kind that is physically kept at the business site, generally local storage. They can be a secondary hard drive, a USB drive, CD/DVD or some kind of RAID device. The keyword is that they are local and as a result will be the fastest to backup and the fastest to restore should something happen. The problem with on-site is that they can easily be stolen as well as destroyed with the rest of your business in the event of that disaster.

An off-site backup is exactly as it sounds, it is stored physically away from the business. This type of backup is becoming more popular with cloud-based backup solutions. Companies like Backblaze, IDrive, and Carbonite make it easy for anyone to back up a computer system. The benefit for off-site is that they are away from your business. Should your business burn down entirely, melting your computers and on-site backup in the fire, then you still have your backups that are stored off-site. The downside to off-site is that it is slower to restore that data as it will only download as fast as your Internet connection will allow.





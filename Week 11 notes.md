# CIT 114 Week 11
## Here are some important thinkgs I learned in Week 11
### Notes 09: Cloud Architecture

#### Well Architected Framework

The AWS Well-Architected Framework helps you understand the pros and cons of decisions you make while building systems on AWS.
By using the Framework you will learn architectural best practices for designing and operating reliable, secure, efficient, and
cost-effective systems in the cloud.

------

 #### Reliatbility

One of the best practices that is identified in the AWS Well-Architected Framework is to plan for failure (or application or workload downtime). One way to do that is to architect your applications and workloads to withstand failure. There are two important factors that cloud architects consider when designing architectures to withstand failure: reliability and availability.

Reliability is the measure of your systems ability to perform its intended function correctly and consistently when it’s expected to. This means the system is available for use and able to operate the workload through its total lifecycle. All apects of the system must be considered including: hardware, firmware, and software. Failure of any one of these impacts the reliabilty of the system.

Reliability should be considered a statistical tool. No system is perfect and there is always the probability that your system will function as intended for a specified period of time.
Should a failure happen, this will affect the mean time between failures (MTBF) is equal to the total time in service divided by the number of failures.

For example, think about a car as a system. It contains an engine, brakes, ignition, and much more. All of the components must work for the entire system to work. If the ignition fails, the car cannot be started and the system has failed. If this has happened only once in the time you own the car, the MTBF is very low and the car is reliable, but if it happens every month, the MTBF is very high and the car is not reliable.

Another metric is the mean time to failure (MTTF) which is the length of time a system is available until it fails. Once it does fail, you need to repair and bring the system back online. The mean time to repair (MTTR) is the amount of time taken to repair a system. The MTBF can be expanded to equal MTTF + MTTR divided by the number of failures.

This creates a failure-repair-restore cycle that:

1.	A system is brought online and is available
2.	A system component then fails, we can now calculate the MTBF
3.	A system component is repaired, we can now calculate the MTTR
4.	A system is brought back online after repair, we can now calculate the MTBF

------

#### Availability

In computing, the term availability is used to describe the period of time when a service is available, as well as the time required by a system to respond to a request made by a user. Availability (also known as service availability) is a commonly used metric to quantitatively measure reliability. Availability is defined as the percentage of time that a workload is available for use. Available for use means that it performs its agreed function when required.

Availability = "Available for Use Time" / "Total Time"

This number the percentage of up-time over a period of a time, normally a year. Common short-hand refers only to the "number of 9's"; for example, "five nines" translates to being 99.999% available. However what does this concept of the 9's mean?

Factors that influence availability include:
   * Fault Tolerance: built in redundancy of a system or application so it can remain operational
   * Scalability: ability to accommodate increase or decrease in capacity usage without changing the design
   * Recoverability: process, policies, and procedures related to restoring a system after system failure

What is High Availability?

High availability (HA) is a quality of a system or component that assures a high level of operational performance for a given period of time. A system can degrade, but still remain available in a HA system. Therefore downtime and required human intervention are minimized.

High availability functions as a failure response mechanism for infrastructure. The way that it works is quite simple conceptually but typically requires some specialized software and configuration.

When setting up robust production systems, minimizing downtime and service interruptions is often a high priority. Regardless of how reliable your systems and software are, problems can occur that can bring down your applications or your servers.

Implementing high availability for your infrastructure is a useful strategy to reduce the impact of these types of events. Highly available systems can recover from server or component failure automatically.

Availability Tiers

|Maximum Unavailability (per year)|Application Categories|
|---|---|
|3 days 15 hours|Batch processing, data extraction, transfer, and load jobs|
|8 hours 45 minutes|Internal tools like knowledge management, project tracking|
|4 hours 22 minutes|Online commerce, point of sale|
|52 minutes|Video delivery, broadcast workloads|
|5 minutes|ATM transactions, telecommunications workloads|

------

Service Level Agreements (SLA)

Now that you know what Reliability and Availability are, all cloud providers have Service Level Agreements (SLA) which define the level of service you can expect from the provider. These lay out metrics by service as well as provide for remedies and penalties should the agreed upon service levels are not achieved. Elements of a SLA include:
  * Provides clear expectations by the provider
  * Metrics that are measured by individual service
  * Availability is provided in percentage per year
  * Penalties are laid out if service levels are not met

AWS Service Level Agreements can be found in the legal section of their site.

------

#### AWS Well-Architected Tool

The AWS Well-Architected Tool (AWS WA Tool) helps you review the state of your workloads and compares them to the latest AWS architectural best practices. The tool is based on the AWS Well-Architected Framework, developed to help cloud architects build secure, high-performing, resilient, and efficient application infrastructure. This Framework provides a consistent approach for customers and partners to evaluate architectures, has been used in tens of thousands of workload reviews conducted by the AWS solutions architecture team, and provides guidance to help implement designs that scale with application needs over time.

To use this free tool, available in the AWS Management Console, just define your workload and answer a set of questions regarding operational excellence, security, reliability, performance efficiency, and cost optimization. The AWS Well-Architected Tool then provides a plan on how to architect for the cloud using established best practices.

AWS WA Tool helps you throughout the product lifecycle by:
   * Assisting with documenting the decisions that you make
   * Providing recommendations for improving your workload based on best practices
   * Guiding you in making your workloads more reliable, secure, efficient, and cost-effective

How it Works

1.	Identify the workload to document. Then answer a series of questions about your architecture
2.	Review your answers against the five pillars established by the Well-Architected Framework that are visually depicted via the icons in the column; 
1.	Operational excellence
2.	Security
3.	Reliability
4.	Performance efficiency
5.	Cost optimization
3.	You can 1) get videos and documentation 2) generate a report that summarizes your workload review, & 3) see the results of reviews in a single dashboard.

------

#### AWS Trusted Advisor

AWS Trusted Advisor is an online tool that provides you real time guidance to help you provision your resources following AWS best practices. Trusted Advisor checks help optimize your AWS infrastructure, increase security and performance, reduce your overall costs, and monitor service limits. Whether establishing new workflows, developing applications, or as part of ongoing improvement, take advantage of the recommendations provided by Trusted Advisor on a regular basis to help keep your solutions provisioned optimally.

AWS Trusted Advisor analyzes your AWS environment and provides best practice recommendations in five categories, which include:
   * Cost Optimization
   * Performance
   * Security
   * Fault Tolerance
   * Service Limits

There are two types of trusted advisor options:
   * Core checks and Recommendations come with all accounts.
   * And full Trusted Advisor for Business and Enterprise support offerings.

AWS Trusted Advisor is not focused on just one service and it is not just a security tool. An AWS Trusted Advisor will tell you how the infrastructure is performing, when security groups have been left open to the world, whether or not you are using fault tolerance, if you are at risk with all everything deployed in an Availability Zone, or if you have resources deployed that you are not using, but are still being charged for.

AWS Basic Support and AWS Developer Support customers get access to 6 security checks (S3 Bucket Permissions, Security Groups - Specific Ports Unrestricted, IAM Use, MFA on Root Account, EBS Public Snapshots, RDS Public Snapshots) and 50 service limit checks. AWS Business Support and AWS Enterprise Support customers get access to all 115 Trusted Advisor checks (14 cost optimization, 17 security, 24 fault tolerance, 10 performance, and 50 service limits) and recommendations. For a complete list of checks and descriptions, explore Trusted Advisor Best Practices.

Access AWS Trusted Advisor from the Management Tools section of the console. The Trusted Advisor provides real-time guidance to help you provision your resources following AWS best practices and to advise you on cost optimization, performance, security, and fault tolerance.

AWS Support Technology

This provides Technology & Tools to Monitor, Manage, and Optimize Your AWS Environment.

There are three main tools to utilize:
   * AWS Personal Health Dashboard
   * AWS Trusted Advisor
   * AWS Health API


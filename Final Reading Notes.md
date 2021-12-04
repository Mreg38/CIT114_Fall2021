# CIT 114 Final Reading Notes

## These notes will be following the topics for the AWS Cloud Practitioner Exam

### 1. Cloud Concepts Overview

## Concepts and Terminology

Cloud - refers to a distinct IT environment that is designed for the purpose of remotely provisioning scalable and measured IT resources. The term originated as a metaphor for the Internet which is, in essence, a network of networks providing remote access to a set of decentralized IT resources.

IT resource - is a physical or virtual IT-related artifact that can be either software based, such as a virtual server or a custom software program, or hardware-based, such as a physical server or a network device.

On-Premise - is another way of stating "on the premises of a controlled IT environment that is not cloud-based." This term is used to qualify an IT resource as an alternative to "cloud-based." An IT resource that is on-premise cannot be cloud-based, and vice-versa. Key points include:
  *	An on-premise IT resource can access and interact with a cloud-based IT resource.
  *	An on-premise IT resource can be moved to a cloud, thereby changing it to a cloud-based IT resource.
  *	Redundant deployments of an IT resource can exist in both on-premise and cloud based environments.

Scaling - the ability of the IT resource to handle increased or decreased usage demands. Types include:
  * Horizontal Scaling - Scaling out and scaling in. The allocating or releasing of IT resources that are of the same type 
  * Vertical Scaling - Scaling up and scaling down. When an existing IT resource is replaced by another with higher or lower capacity.

Needs for IT Specialists:
  * Data Overload: Businesses need to process huge amounts of data. This requires large amounts of processing power, sophisticated software and human analytical skills.
  * Mobile and Wireless Usages: More employers are offering remote work options that require smartphones, tablets and laptops with wireless hotspots and roaming ability.
  * Cloud Services: Many businesses no longer operate their own “server farms” to store massive amounts of data. Many businesses now work with cloud services—third-party hosting platforms that maintain that data.
  * Bandwidth for Video: Videoconferencing solutions have become more and more popular, so more network bandwidth is needed to support them sufficiently.

4 Pillars of IT Frame work:
  * Infrastructure - Defined broadly as a set of information technology (IT) components that are the foundation of an IT service; typically physical components such as computer and networking hardware and facilities), but also various software and network components.
  * Development - Development is a process of writing and maintaining source code for software applications or frameworks. It involves all phases of the software development life cycle, including:
       - Conceptualizing software
       - Defining requirements
       - Designing how it will work
       - Programming it
       - Documenting its functionality
       - Testing against the requirements
       - Bug fixing any issues 
  * Security - IT security is a set of cybersecurity strategies that prevents unauthorized access to organizational assets such as computers, networks, software, and data. It maintains the integrity and confidentiality of sensitive information, blocking the access of hackers.
  * Data - Data is represented through quantities, characters, or symbols on which operations are performed by a computer are stored and recorded on magnetic, optical, or mechanical recording media, and transmitted in the form of digital electrical signals.

Basic hardware components of a modern personal computer, include
  * Motherboard
  * Central Processing Unit (CPU)
  * Random Access Memory (RAM)
  * Storage Drives
  * Expansion Cards 
      - Graphic Cards (GPU)
      - Audio Cards
      - Networking Components
  * Cooling
  * Power Supply
  * Case
  * Input & Output Devices
  * Peripherals

Business Drivers:
Capacity Planning - The process of determining and fulfilling future demands of an organization's IT resources, products, and services.
Different capacity planning strategies exist:
  * Lead Strategy - adding capacity to an IT resource in anticipation of demand
  * Lag Strategy - adding capacity when the IT resource reaches its full capacity
  * Match Strategy - adding IT resource capacity in small increments, as demand increases
Cost Reduction - Two costs need to be accounted for: the cost of acquiring new infrastructure, and the cost of its ongoing ownership. Operational overhead represents a considerable share of IT budgets, often exceeding up-front investment costs.
Common forms of infrastructure-related operating overhead include the following:
  * technical personnel required to keep the environment operational
  * upgrades and patches that introduce additional testing and deployment cycles
  * utility bills and capital expense investments for power and cooling
  * security and access control measures that need to be maintained and enforced to protect infrastructure resources
  * administrative and accounts staff that may be required to keep track of licenses and support arrangements
Organizational Agility - Businesses need the ability to adapt and evolve to successfully face change caused by both internal and external factors. Organizational agility is the measure of an organization's responsiveness to change.

------

## Goals and Benefits

Reduced Investments and Proportional Costs

The most common economic rationale for investing in cloud-based IT resources is in the reduction or outright elimination of up-front IT investments, namely hardware and software purchases and ownership costs. A cloud's Measured Usage characteristic represents a feature-set that allows measured operational expenditures (directly related to business performance) to replace anticipated capital expenditures. This is also referred to as proportional costs.

Common measurable beneﬁts to cloud consumers include:
  * On-demand access to pay-as-you-go computing resources on a short-term basis (such as processors by the hour), and the ability to release these computing resources when they are no longer needed.
  * The perception of having unlimited computing resources that are available on demand, thereby reducing the need to prepare for provisioning.
  * The ability to add or remove IT resources at a ﬁne-grained level, such as modifying available storage disk space by single gigabyte increments.
  * Abstraction of the infrastructure so applications are not locked into devices or locations and can be easily moved if needed.

Increased Scalability

By providing pools of IT resources, along with tools and technologies designed to leverage them collectively, clouds can instantly and dynamically allocate IT resources to cloud consumers, on-demand or via the cloud consumer's direct conﬁguration. This empowers cloud consumers to scale their cloud-based IT resources to accommodate processing ﬂuctuations and peaks automatically or manually. Similarly, cloud-based IT resources can be released (automatically or manually) as processing demands decrease.

Increased Availability and Reliability

The availability and reliability of IT resources are directly associated with tangible business benefits. Outages limit the time an IT resource can be "open for business" for its customers, thereby limiting its usage and revenue generating potential. Runtime failures that are not immediately corrected can have a more significant impact during high-volume usage periods. Not only is the IT resource unable to respond to customer requests, its unexpected failure can decrease overall customer confidence.

------

## Risks and Challenges

## AWS Perspective

## Software as a Service (SaaS)

------

### 2. Cloud Economics, Billing & Support

## AWS Pricing



## Total Cost of Ownership



------

### 3. Cloud Global Infrastructure

Computing w/AWS

AWS Global Infrastructure Terminology

AWS Global Infrastructure

Regions and Availability Zones

AWS Foundational Services

------

### 4. Cloud Security

## Intro to AWS SErcurity

## AWS Shared Security Model

## AWS Sercurity Best Practices

## AWS IAM (6.06 thru 6.09)

## AWS Services for Cloud Security (6.12 thru 6.15)

------

### 5. Networking & Content Delivery

## Introduction to Networking (7.01 thru 7.06)

## AWS VPC (7.07 thru 7.11)

## VPC Networking (7.12 thru 7.19)

## VPC Security (7.20, 7.21)

## AWS Networking Services (7.22, 7.23)

------

### 6. Compute

## Available Operatoing Systems at AWS

## AWS Compute Services + Choosing the Right Service

## Virtual Machines (inc. EC2)

## Containers (inc. Docker & Kubernetes)

## Serverless (inc. AWS Lambda)

## PaaS (inc. AWS Elastic Beanstalk)

------

### 7. Storage

## AWS Storage Services

## S3

## Glacier

## EBS

## EFS

------

### 8. Databases

## AWS Databases

## AWS Relational Database Services

## AWS Dynamo DB

## AWS Redshift

## AWS Aurora

------

### 9. Cloud Architecture

## Document: AWS Well Architected Framework

## Reliability

## Availability

## AWS Trusted Advisor


------

### 10. Automatic Scaling & Monitoring

## AWS CloudWatch

## Amazon EC2 AutoScaling

## Chapter 5 via O'Reilly: Planning for Scale & Resiliency

# CIT 114 Final Reading Notes

## These notes will be following the topics for the AWS Cloud Practitioner Exam

### 1. Cloud Concepts Overview (Mix of first few weeks)

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

## Goals and Benefits (Week 2 - 2.1 - 2.17)

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

## Risks and Challenges (Week 2 - 2.1 to 2.17)

Increased Security Vulnerabilities

The moving of business data to the cloud means that the responsibility over data security becomes shared with the cloud provider. The remote usage of IT resources requires an expansion of trust boundaries by the cloud consumer to include the external cloud. It can be difﬁcult to establish a security architecture that spans such a trust boundary without introducing vulnerabilities, unless cloud consumers and cloud providers happen to support the same or compatible security frameworks - which is unlikely with public clouds.

Reduced Operational Governance Control

Cloud consumers are usually allotted a level of governance control that is lower than that over on-premise IT resources. This reduced level of governance control can introduce risks associated with how the cloud provider operates its cloud, as well as the external connections that are required to communicate between the cloud and the cloud consumer. Consider the following examples:
  * An unreliable cloud provider may not maintain the guarantees it makes in the SLAs that were published for its cloud services. This can jeopardize the quality of the cloud consumer solutions that rely on these cloud services.
  * Longer geographic distances between the cloud consumer and cloud provider can require additional network hops that introduce ﬂuctuating latency and potential bandwidth constraints.

Limited Portability Between Cloud Providers

Due to a lack of established industry standards within the cloud computing industry, public clouds are commonly proprietary to various extents. For cloud consumers that have custom-built solutions with dependencies on these proprietary environments, it can be challenging to move from one cloud provider to another.

Multi-Regional Regulatory and Legal Issues

Third-party cloud providers will frequently establish data centers in affordable or convenient geographical locations. Cloud consumers will often not be aware of the physical location of their IT resources and data when hosted by public clouds. For some organizations, this can pose serious legal concerns pertaining to industry or government regulations that specify data privacy and storage policies. For example, some UK laws require personal data belonging to UK citizens to be kept within the United Kingdom.

Another potential legal issue pertains to the accessibility and disclosure of data. Countries have laws that require some types of data to be disclosed to certain government agencies or to the subject of the data. For example, a European cloud consumer's data that is located in the U.S. can be more easily accessed by government agencies (due to the U.S. Patriot Act) when compared to data located in many European Union countries.

Most regulatory frameworks recognize that cloud consumer organizations are ultimately responsible for the security, integrity, and storage of their own data, even when it is held by an external cloud provider.

## AWS Perspective (Week 2 - 2.1 to 2.17)

1. Trade capital expense for variable expense

Instead of having to invest heavily in data centers and servers before you know how you’re going to use them, you can only pay when you consume computing resources, and only pay for how much you consume.

2. Benefit from massive economies of scale

By using cloud computing, you can achieve a lower variable cost than you can get on your own. Because usage from hundreds of thousands of customers are aggregated in the cloud, providers such as Amazon Web Services can achieve higher economies of scale which translates into lower pay as you go prices.

3. Stop guessing capacity

Eliminate guessing on your infrastructure capacity needs. When you make a capacity decision prior to deploying an application, you often either end up sitting on expensive idle resources or dealing with limited capacity. With Cloud Computing, these problems go away. You can access as much or as little as you need, and scale up and down as required with only a few minutes notice.

4. Increase speed and agility

In a cloud computing environment, new IT resources are only ever a click away, which means you reduce the time it takes to make those resources available to your developers from weeks to just minutes. This results in a dramatic increase in agility for the organization, since the cost and time it takes to experiment and develop is significantly lower.

5. Stop spending money on running and maintaining data centers

Focus on projects that differentiate your business, not the infrastructure. Cloud computing lets you focus on your own customers, rather than on the heavy lifting of racking, stacking and powering servers.

6. Go global in minutes

Easily deploy your application in multiple regions around the world with just a few clicks. This means you can provide a lower latency and better experience for your customers simply and at minimal cost.

## Software as a Service (SaaS) (Week 2 - 2.1 to 2.17)

Software as a service (SaaS) allows users to connect to and use cloud-based apps over the Internet. Common examples are email, calendaring, and office tools (such as Microsoft Office 365).

SaaS provides a complete software solution that you purchase on a pay-as-you-go basis from a cloud service provider.  You rent the use of an app for your organization, and your users connect to it over the Internet, usually with a web browser. All of the underlying infrastructure, middleware, app software, and app data are located in the service provider’s data center. The service provider manages the hardware and software, and with the appropriate service agreement, will ensure the availability and the security of the app and your data as well. SaaS allows your organization to get quickly up and running with an app at minimal upfront cost.

Common Scenarios

If you’ve used a web-based email service such as Outlook, Hotmail, or Yahoo! Mail, then you’ve already used a form of SaaS. With these services, you log into your account over the Internet, often from a web browser. The email software is located on the service provider’s network, and your messages are stored there as well. You can access your email and stored messages from a web browser on any computer or Internet-connected device.

The previous examples are free services for personal use. For organizational use, you can rent productivity apps, such as email, collaboration, and calendaring; and sophisticated business applications such as customer relationship management (CRM), enterprise resource planning (ERP), and document management. You pay for the use of these apps by subscription or according to the level of use.

Advantages of SaaS

Gain access to sophisticated applications:

To provide SaaS apps to users, you don’t need to purchase, install, update, or maintain any hardware, middleware, or software. SaaS makes even sophisticated enterprise applications, such as ERP and CRM, affordable for organizations that lack the resources to buy, deploy, and manage the required infrastructure and software themselves.

Pay only for what you use:

You also save money because the SaaS service automatically scales up and down according to the level of usage.
Use free client software. Users can run most SaaS apps directly from their web browser without needing to download and install any software, although some apps require plugins. This means that you don’t need to purchase and install special software for your users.

Mobilize your workforce easily:

SaaS makes it easy to “mobilize” your workforce because users can access SaaS apps and data from any Internet-connected computer or mobile device. You don’t need to worry about developing apps to run on different types of computers and devices because the service provider has already done so. In addition, you don’t need to bring special expertise onboard to manage the security issues inherent in mobile computing. A carefully chosen service provider will ensure the security of your data, regardless of the type of device consuming it.

Access app data from anywhere:

With data stored in the cloud, users can access their information from any Internet-connected computer or mobile device. And when app data is stored in the cloud, no data is lost if a user’s computer or device fails.

------

### 2. Cloud Economics, Billing & Support (Week 4 - 4.1 to 4.26)

## AWS Pricing

AWS offers pay-as-you-go (on demand), reservation-based, and bulk-use (pay less when you use more) payment models; this enables us to obtain the best return on your investment for each specific use case. AWS services do not have complex dependencies or licensing requirements, so you can get exactly what you need to build innovative, costeffective solutions using the latest technology. 

How do you pay for AWS?

Pay-as-you-go:

AWS pricing is similar to how you pay for utilities like water and electricity. You only pay for the services you consume, and once you stop using them, there are no additional costs or termination fees.

Save when you reserve:

For certain services like Amazon EC2 and Amazon RDS, you can invest in reserved capacity. With Reserved Instances, you can save up to 75% over equivalent on-demand capacity. When you buy Reserved Instances, the larger the upfront payment, the greater the discount. 

Pay less by using more:

With AWS, you can get volume based discounts and realize important savings as your usage increases. For services such as S3 and data transfer OUT from EC2, pricing is tiered, meaning the more you use, the less you pay per GB. In addition, data transfer IN is always free of charge. As a result, as your AWS usage needs increase, you benefit from the economies of scale that allow you to increase adoption and keep costs under control.

Key Principles of Pricing

1. There are three fundamental drivers of cost with AWS:
  * Compute
  * Storage
  * Outbound data transfer

2. Start early with cost optimization:

Adopting cloud services is not just a technical evolution. It also requires changes to how organizations operate. As you move from IT being treated as a capital investment that happens periodically to a world where pricing is closely tied to efficient use of resources, it pays to understand what drives cloud pricing so you can build a strategy for optimizing it.

3. Maximize the power of flexibility:

AWS services are priced independently and transparently, so you can choose and pay for exactly what you need and no more. No minimum commitments or long-term contracts are required unless you choose to save money through a reservation model. By paying for services on an as-needed basis, you can redirect your focus to innovation and invention, reducing procurement complexity and enabling your business to be fully elastic.

4. Use the right pricing model for the job:

AWS offers several pricing models depending on product. These include:
  * On Demand means you pay for compute or database capacity with no long-term commitments or upfront payments.
  * Dedicated Instances (available with Amazon Elastic Compute Cloud. (Amazon EC2)) run in a virtual private cloud (VPC) on hardware that’s dedicated to a single customer.
  * Spot Instances are an Amazon EC2 pricing mechanism that lets you purchase spare computing capacity with no upfront commitment at discounted hourly rates.
  * Reservations provide you with the ability to receive a greater discount, up to 75 percent, by paying for capacity ahead of time. More detail is provided in the section, “Optimizing costs with reservations.” Reservation options include: 
    - Amazon EC2 Reserved Instances
    - Amazon DynamoDB Reserved Capacity
    - Amazon ElastiCache Reserved Nodes
    - Amazon Relational Database Service Reserved Instances
    - Amazon Redshift Reserved Nodes

Free Tier + Undrstanding the Free Tier

For Rio Hondo:

|Resource|Description|
|---|---|
|AWS Credits|$25 in credits for your normal AWS account, if requested|
|AWS Educate|$100 in credits for a starter account and access to classrooms with additional credits|
|AWS Training|Access to AWS Technical Essentials Training Course and free access to labs|
|Content|1) Ability to select personalized learning pathway with 30+ hours of content per path. 2) Earn digital badges that showcase cloud skills. 3) Free access to AWS content for homework, labs, or self-study|
|Collaboration|1) Student Portal access. 2) Student Portfolio to store developed projects in one place. 3) Access to the AWS Job Board and job postings.|

Otherwise:

You can test-drive some AWS services free of charge, within certain usage limits. AWS calls this the AWS Free Tier. The free tier is designed to give you hands-on experience with a range of AWS services at no charge. When you create an AWS account, you are automatically signed up for the free tier for 12 months. Your free tier eligibility expires at the end of the 12-month period. When your free tier expires, AWS starts charging the regular rates for any AWS services and resources that you are using. 

1) 12 Months Free – These tier offers include 12 months free usage following your initial sign-up date to AWS. When your 12 month free usage term expires, or if your application use exceeds the tiers, you simply pay standard, pay-as-you-go service rates.
2) Always Free – These free tier offers do not expire and are available to all AWS customers.
3) Trials – These offers are short term free trials starting from date you activate a particular service. Once the trial period expires, you simply pay standard, pay-as-you-go service rates.

Services with No Charge

  * Amazon Virtual Private Cloud (Amazon VPC) enables you to provision a logically isolated section of the AWS Cloud where you can launch AWS resources in a virtual network that you define.
  * AWS Identity and Access Management (IAM) controls your users’ access to AWS services and resources.
  * Consolidated Billing is a billing feature in AWS Organizations to consolidate payment for multiple AWS accounts or multiple Amazon Internet Services Private Limited (AISPL) accounts*. Consolidated billing provides: 
    - One bill for multiple accounts
    - The ability to easily track each account’s charges
    - The opportunity to decrease charges as a result of volume pricing discounts from combined usage.
    - And you can consolidate all of your accounts using Consolidated Billing and get tiered benefits.
  * AWS Elastic Beanstalk is an even easier way for you to quickly deploy and manage applications in the AWS Cloud.
  * AWS CloudFormation gives developers and systems administrators an easy way to create a collection of related AWS resources and provision them in an orderly and predictable fashion.
  * Automatic Scaling automatically adds or removes resources according to conditions you define. The resources you are using increase seamlessly during demand spikes to maintain performance and decrease automatically during demand lulls to minimize costs.
  * AWS OpsWorks is an application management service that makes it easy to deploy and operate applications of all shapes and sizes.

## Total Cost of Ownership (Week 4 - 4.1 to 4.26)

IT Infrastructure

Information technology (IT) infrastructure are the components required to operate and manage enterprise IT environments. IT infrastructure can be deployed within a cloud computing system, or within an organization's own facilities.

These components include hardware, software, networking components, an operating system (OS), and data storage, all of which are used to deliver IT services and solutions. IT infrastructure products are available as downloadable software applications that run on top of existing IT resources—like software-defined storage—or as online solutions offered by service providers—like Infrastructure-as-a-Service (IaaS).

Components:

Hardware - includes servers, datacenters, personal computers, routers, switches, and other equipment. The facilities that house, cool, and power a datacenter could also be included as part of the infrastructure.

Software - refers to the applications used by the business, such as web servers, content management systems, and the OS—like Linux (Links to an external site.)®. The OS is responsible for managing system resources and hardware, and makes the connections between all of your software and the physical resources that do the work.

Network - interconnected network components enable network operations, management, and communication between internal and external systems. The network consists of internet connectivity, network enablement, firewalls and security, as well as hardware like routers, switches, and cables.

Types of IT infrastructure:

Traditional infrastructure - With a traditional infrastructure, the components—like datacenters, data storage, and other equipment—are all managed and owned by the business within their own facilities. Traditional infrastructure is often thought of as expensive to run and requires large amounts of hardware, like servers, as well as power and physical space.

Cloud infrastructure - describes the components and resources needed for cloud computing. You can create a private cloud by building it yourself using resources dedicated solely to you. Or you can use a public cloud by renting cloud infrastructure from a cloud provider like Alibaba, Amazon, Google, IBM, or Microsoft. And by incorporating some degree of workload portability, orchestration, and management across multiple clouds you can create a hybrid cloud

What is the Total Cost of Ownership?

Total cost of ownership, or TCO, is a formula that assesses direct and indirect costs and benefits related to the purchase of any IT component. The goal is a final figure that will reflect the true purchase price, all things considered.

TCO models are domain-dependent, then defining your own model will be part of the process. The best approach is to consider a list of attributes for the model, and then the degree to which these properties are relevant to your problem domain or enterprise. This will provide you with the ability to understand what benefits of cloud computing are most relevant to your business, and thus gain a true idea of the TCO.

These properties include, but are not limited to:
  * Existing infrastructure in place. Those 10 million dollars you spent on a new data center, and servers to fill it, can’t be recovered. Leveraging cloud as a replacement for existing infrastructure means you have to factor the cost of sidelining the existing assets.
  * Existing skills and humans. In moving to cloud-based platforms, there are new skills and talent required that are likely different from the skills and talent you have in place. How much will this part of the transition cost?
  * Moreover, what’s the difference in costs from pre-cloud to post-cloud? Cost of migration to cloud platforms. The amount of money it will take to move some applications and data to cloud-based platforms, including redoing aspects of the applications to better support cloud.
  * Cost of cloud services when in operations. This includes the fees paid to the cloud provider, in the case of using public clouds, over a duration of time and should include a changing operational load.
  * Value of agility (including time-to-market). Or, the value that the company places on the ability to shift or align quickly to the changing needs of the business. This should be considered around points of value delivered, such as the ability to quickly stand up cloud-based systems in support of a strategic acquisition, or to quickly scale up to higher storage capabilities in support of expanding R&D to new and emerging product lines.
  * Value of avoiding future capital expenditures. The hardware and software budgets of the past get a complete makeover, with most traditional purchases being greatly reduced or eliminated altogether. This gets to the whole opex versus capex type of value.
  * Cost of risk around compliance issues. If you’re in the healthcare or finance verticals, you’re already aware of the issues around compliance with rules and regulations. When moving to cloud, you could be adding or removing risk of non-compliance. These have costs to consider, and thus should be baked into the TCO calculation.

How is Total Cost of Ownership Calculated?

TCO is a financial estimate that helps enterprise managers determine both direct and indirect costs of a product or system, such as AWS. This management accounting concept can be used to understand the big, long-term picture of exactly how much AWS will cost (or more accurately, save) your organization. Considerations for TCO extend beyond just the initial purchase price or implementation costs and account for the full cost of an asset over its life, which aren’t always reflected in upfront pricing.

Components of Total Cost for Technology
  * Hardware acquisition
  * Software acquisition
  * Infrastructure
  * Downtime
  * Installation
  * Maintenance
  * Training
  * Support
  * Space
  * Electricity

------

### 3. Cloud Global Infrastructure (Week 15 15.01 to 15.12)

Computing w/AWS

Using cloud for things such as data back up or recovery, email, virtual desktops, software development & testing, customer facing web applications to make a business more agile, reduce cost, instantly scale and deploy globally in minutes.

AWS Global Infrastructure Terminology

AWS Regions - are separate geographic areas that AWS uses to house its infrastructure. These are distributed around the world so that customers can choose a region closest to them in order to host their cloud infrastructure there. The closer your region is to you, the better, so that you can reduce network latency as much as possible for your end-users. You want to be near the data centers for fast service.

Best practices for choosing AWS Regions

In general, try to follow these best practices when you choose a region, to help ensure top performance and resilience:
  * Proximity: Choose a region closest to your location and your customers’ location to optimize network latency.
  * Services: Try and think about what are your most needed services. Usually, the newest services start on a few main regions then pop up in other regions later.
  * Cost: Certain regions will cost more than others, so use built-in AWS calculators to do rough cost estimates to inform your choices.
  * Service Level Agreement (SLA): Just as with cost, your SLA details will vary by region, so be sure to be aware of what your needs are and if they’re being met.
  * Compliance: You may need to meet regulatory compliance needs such as GDPR by hosting your deployment in a specific — or multiple regions.

AWS Availability Zone (AZ) - is the logical building block that makes up an AWS Region. There are currently 76 AZs, which are isolated locations— data centers — within a region. Each region has multiple AZs and when you design your infrastructure to have backups of data in other AZs you are building a very efficient model of resiliency, i.e. a core concept of cloud computing.

AWS Infrastructure Features:

First, AWS Infrastructure is elastic and scalable. This means resources can dynamically adjust to increases or decreases in capacity requirements. It can also rapidly adjust to accommodate growth.

Second, this infrastructure is fault tolerant, which means it has built-in component redundancy which enables it to continue operations despite a failed component.

AWS Global Infrastructure

The AWS Global Cloud Infrastructure is the most secure, extensive, and reliable cloud platform, offering over 200 fully featured services from data centers globally. Whether you need to deploy your application workloads across the globe in a single click, or you want to build and deploy specific applications closer to your end-users with single-digit millisecond latency, AWS provides you the cloud infrastructure where and when you need it.

With millions of active customers and tens of thousands of partners globally, AWS has the largest and most dynamic ecosystem. Customers across virtually every industry and of every size, including start-ups, enterprises, and public sector organizations, are running every imaginable use case on AWS.

The AWS Cloud spans 81 Availability Zones within 25 geographic regions around the world, with announced plans for 27 more Availability Zones and 9 more AWS Regions in Australia, Canada, India, Indonesia, Israel, New Zealand, Spain, Switzerland, and United Arab Emirates (UAE). 

Regions and Availability Zones

AWS has the concept of a Region, which is a physical location around the world where we cluster data centers. We call each group of logical data centers an Availability Zone. Each AWS Region consists of multiple, isolated, and physically separate AZs within a geographic area. Unlike other cloud providers, who often define a region as a single data center, the multiple AZ design of every AWS Region offers advantages for customers. Each AZ has independent power, cooling, and physical security and is connected via redundant, ultra-low-latency networks. AWS customers focused on high availability can design their applications to run in multiple AZs to achieve even greater fault-tolerance. AWS infrastructure Regions meet the highest levels of security, compliance, and data protection.

An Availability Zone (AZ) is one or more discrete data centers with redundant power, networking, and connectivity in an AWS Region. AZs give customers the ability to operate production applications and databases that are more highly available, fault tolerant, and scalable than would be possible from a single data center. All AZs in an AWS Region are interconnected with high-bandwidth, low-latency networking, over fully redundant, dedicated metro fiber providing high-throughput, low-latency networking between AZs. All traffic between AZs is encrypted. The network performance is sufficient to accomplish synchronous replication between AZs. AZs make partitioning applications for high availability easy. If an application is partitioned across AZs, companies are better isolated and protected from issues such as power outages, lightning strikes, tornadoes, earthquakes, and more. AZs are physically separated by a meaningful distance, many kilometers, from any other AZ, although all are within 100 km (60 miles) of each other.

AWS Foundational Services

Compute

Compute services help you make the most of your data. They support research and big data processing. AWS compute services cover virtual machines, containers, serverless computing, and more.

For example, Munich Leukemia Laboratory uses AWS for genome sequencing (Links to an external site.); using Amazon Elastic Compute Cloud (Amazon EC2), they were able to process sequencing runs in 30-40 minutes, versus 10-12 hours before the cloud.

Storage

AWS storage solutions provide reliable, scalable, and secure storage for backup, disaster recovery, and business continuity. 

For example, the Smithsonian Institution shared over 2.8 million images stored in Amazon Simple Storage Service (Amazon S3) (Links to an external site.) for public analysis and use.

Databases

WS databases are built for different data models and use cases and offer speed, reliability, availability, and security.

For example, the Pokemon Company migrated to AWS managed database services (Links to an external site.) in order to free up time and resources while improving game play.

Networking

AWS networking and content delivery are designed to ensure that AWS has the networking capabilities required to run any workload in the cloud with security, availability, performance, global coverage, and manageability.

------

### 4. Cloud Security (Week 6 6.01 to 6.16)

## Intro to AWS Security

The AWS infrastructure has been architected to be one of the most flexible and secure cloud computing environments available today. It is designed to provide an extremely scalable, highly reliable platform that enables customers to deploy applications and data quickly and securely.

This infrastructure is built and managed not only according to security best practices and standards, but also with the unique needs of the cloud in mind. AWS uses redundant and layered controls, continuous validation and testing, and a substantial amount of automation to ensure that the underlying infrastructure is monitored and protected 24x7. AWS ensures that these controls are replicated in every new data center or service.

All AWS customers benefit from a data center and network architecture built to satisfy the requirements of our most security-sensitive customers. This means that you get a resilient infrastructure, designed for high security, without the capital outlay and operational overhead of a traditional data center.

AWS operates under a shared security responsibility model, where AWS is responsible for the security of the underlying cloud infrastructure and you are responsible for securing workloads you deploy in AWS (Figure 1). This gives you the flexibility and agility you need to implement the most applicable security controls for your business functions in the AWS environment. You can tightly restrict access to environments that process sensitive data, or deploy less stringent controls for information you want to make public.

## AWS Shared Security Model

Security and Compliance is a shared responsibility between AWS and the customer. This shared model can help relieve the customer’s operational burden as AWS operates, manages and controls the components from the host operating system and virtualization layer down to the physical security of the facilities in which the service operates. The customer assumes responsibility and management of the guest operating system (including updates and security patches), other associated application software as well as the configuration of the AWS provided security group firewall. Customers should carefully consider the services they choose as their responsibilities vary depending on the services used, the integration of those services into their IT environment, and applicable laws and regulations. The nature of this shared responsibility also provides the flexibility and customer control that permits the deployment. As shown in the chart below, this differentiation of responsibility is commonly referred to as Security “of” the Cloud versus Security “in” the Cloud.

AWS is responsible for protecting the infrastructure that runs all of the services offered in the AWS Cloud. This infrastructure is composed of the hardware, software, networking, and facilities that run AWS Cloud services. This includes:
  * Physical security of data centers with controlled, need-based access; located in nondescript facilities, with 24/7 security guards; two-factor authentication; access logging and review; video surveillance; and disk degaussing and destruction.
  * Hardware infrastructure, such as servers, storage devices, and other appliances that AWS relies on.
  * Software infrastructure, which hosts operating systems, service applications, and virtualization software.
  * Network infrastructure, such as routers, switches, load balancers, firewalls, and cabling. AWS also continuously monitors the network at external boundaries, secures access points, and provides redundant infrastructure with intrusion detection.

While the cloud infrastructure is secured and maintained by AWS, customers are responsible for security of everything they put in the cloud.

The customer is responsible for what is implemented by using AWS services and for the applications that are connected to AWS. The security steps that you must take depend on the services that you use and the complexity of your system. Customer responsibilities include selecting and securing any instance operating systems, securing the applications that are launched on AWS resources, security group configurations, firewall configurations, network configurations, and secure account management.

The selection made by the customer determines the amount of configuration work the customer must perform as part of their security responsibilities. 

## AWS Security Best Practices

  * Know the AWS Shared Responsibility Model
  * Understanding the AWS Secure Global Infrastructure
    - Sharing Security Responsibility for AWS Services
    - Using the Trusted Advisor Tool
  * Manage AWS Accounts, IAM Users, Groups, and Roles
    - Strategies for Using Multiple AWS Accounts
    - Managing IAM Users
    - Managing IAM Groups
    - Managing AWS Credentials

## AWS IAM (6.06 thru 6.09)

AWS Identity and Access Management (IAM) is a web service that helps you securely control access to AWS resources for your users. You use IAM to control who can use your AWS resources (authentication) and what resources they can use and in what ways (authorization).

When you first create an AWS account, you begin with a single sign-in identity that has complete access to all AWS services and resources in the account. This identity is called the AWS account root user and is accessed by signing in with the email address and password that you used to create the account.

Authorization is the process of determining what permissions a user, service or application should be granted. After a user has been authenticated, they must be authorized to access AWS services.

By default, IAM users do not have permissions to access any resources or data in an AWS account. Instead, you must explicitly grant permissions to a user, group, or role by creating a policy.

To assign permission to a user, group or role, you must create an IAM policy (or find an existing policy in the account). There are no default permissions. All actions in the account are denied to the user by default (implicit deny) unless those actions are explicitly allowed. Any actions that you do not explicitly allow are denied. Any actions that you explicitly deny are always denied.

The principle of least privilege is an important concept in computer security. It promotes that you grant only the minimal user privileges needed to the user, based on the needs of your users. When you create IAM policies, it is a best practice to follow this security advice of granting least privilege. Determine what users need to be able to do and then craft policies for them that let the users perform only those tasks. Start with a minimum set of permissions and grant additional permissions as necessary. Doing so is more secure than starting with permissions that are too broad and then later trying to lock down the permissions granted.

## AWS Services for Cloud Security (6.12 thru 6.15)

  * AWS Service Catalog - allows organizations to create and manage catalogs of IT services that are approved for use on AWS. These IT services can include everything from virtual machine images, servers, software, and databases to complete multi-tier application architectures.
  * AWS Web Application Firewall (WAF) - helps protect your web applications or APIs against common web exploits that may affect availability, compromise security, or consume excessive resources. This differs from AWS Shield in that it operates on application layer (Layer 7) of the OSI model and protects against attacks such as SQL injection or cross-site scripting.
  * Amazon Macie - is a fully managed data security and data privacy service that uses machine learning and pattern matching to discover and protect your sensitive data in AWS. It can help you proactively identify and protect personally identifiable information (PII) and know when it moves.
  * Amazon Inspector - is an automated security assessment service that helps improve the security and compliance of applications deployed on AWS. Amazon Inspector automatically assesses applications for exposure, vulnerabilities, and deviations from best practices. It can help you validate you are adhering to standards.
  * Amazon GuardDuty - is an intelligent threat detection service that continuously monitors for malicious activity and unauthorized behavior to protect your AWS accounts and workloads.

------

### 5. Networking & Content Delivery (Week 7 - 7.01 to 7.23)

## Introduction to Networking (7.01 thru 7.06)

In the broadest terms, people often view the Internet as a cloud. You put your data in one place, and it comes out the place you want it to on the other side, with what happens in between obscured in the fog.

In reality the internet is tens of thousands kilometres of fiber optic cable, hundreds of thousands to millions of kilometres of copper wire, and hardware and software connecting them all together in a redundant, fast, and self-sufficient network. But not to worry, it’s not that bad: you only have to worry about a very small portion of the network, you can let someone else worry about the rest.

Computer Network - It is the interconnection of multiple devices, generally termed as Hosts connected using multiple paths for the purpose of sending/receiving data or media. There are also multiple devices or mediums which helps in the communication between two different devices which are known as Network devices. Ex: Router, Switch, Hub, Bridge.

OSI (Open Systems Interconnection) - It is a reference model that specifies standards for communications protocols and also the functionalities of each layer.

The OSI Model layers are as follows: (Anagram: All People Seem To Need Data Processing)

  * Layer 7 - Application - The application layer is the OSI layer closest to the end user, which means both the OSI application layer and the user interact directly with the software application.
  * Layer 6 - Presentation - The presentation layer establishes context between application-layer entities, in which the application-layer entities may use different syntax and semantics if the presentation service provides a mapping between them.
  * Layer 5 - Session - The session layer controls the dialogues (connections) between computers. It establishes, manages and terminates the connections between the local and remote application.
  * Layer 4 - Transport - The transport layer provides the functional and procedural means of transferring variable-length data sequences from a source to a destination host, while maintaining the quality of service functions.
  * Layer 3 - Network - The network layer provides the functional and procedural means of transferring variable length data sequences (called packets) from one node to another connected in "different networks".
  * Layer 2 - Data Link - The data link layer provides node-to-node data transfer—a link between two directly connected nodes
  * Layer 1 - Physical - Responsible for the transmission and reception of unstructured raw data between a device and a physical transmission medium.

Protocol - is the set of rules or algorithms which define the way how two entities can communicate across the network and there exists different protocol defined at each layer of OSI model. Few of such protocols are TCP, IP, UDP, ARP, DHCP, FTP and so on.

Unique Identifiers of Network

Host name - Each device in the network is associated with a unique device name

IP Address (Internet Protocol address) - Also, know as Logical Address, is the network address of the system across the network. To identify each device in the world-wide-web, Internet Assigned Numbers Authority (IANA) assigns IPv4 (Version 4) address as a unique identifier for each device on the Internet. However there is also an IPv6 (Version 6) scheme available that has more addresses available.

Classless Inter-Domain Routing (CIDR) - A common method to describe networks is Classless Inter-Domain Routing (CIDR). The CIDR address is expressed as follows:
  * An IP address (which is the first address of the network)
  * Next, a slash character (/)
  * Finally, a number that tells you how many bits of the routing prefix must be fixed or allocated for the network identifier

MAC Address (Media Access Control address) - Also known as physical address, is the unique identifier of each host and is associated with the NIC (Network Interface Card). MAC address is assigned to the NIC at the time of manufacturing.

Port - can be referred to as a logical channel through which data can be sent/received to an application. Any host may have multiple applications running, and each of this application is identified using the port number on which they are running on.

Port number is a 16-bit integer, hence we have 216 ports available which are categorized as shown below:
  * Well known Ports 0–1023
  * Registered Ports 1024–49151
  * Ephemeral Ports 49152–65535

Number of ports: 65,536

Range: 0–65535

Socket - The unique combination of IP address and Port number together.

DNS Server (Domain Name System) - basically a server which translates web addresses or URL (ex: www.google.com) into their corresponding IP addresses. We don’t have to remember all the IP addresses of each and every website.

ARP (Address Resolution Protocol) - It is used to convert the IP address to its corresponding Physical Address (i.e. MAC Address). ARP is used by the Data Link Layer to identify the MAC address of the Receiver’s machine.

RARP (Reverse Address Resolution Protocol) - provides the IP address of the device given a physical address as input. But RARP has become obsolete since the time DHCP has come into the picture.

Internet - it is a global network of smaller networks interconnected using communication protocols that are standardized. The Internet standards describe a framework known as the Internet protocol suite. This model divides methods into a layered system of protocols.

These layers are as follows:
1.	Application layer (highest) — concerned with the data(URL, type, etc), where HTTP, HTTPS, etc comes in.
2.	Transport layer — responsible for end-to-end communication over a network.
3.	Network layer — provides a data route.

World Wide Web - is a subset of the internet. It’s a system of Internet servers that support specially formatted documents. The documents are formatted in a markup language called HTML(that supports links, multimedia, etc). These documents are interlinked using hypertext links and are accessible via the Internet.

To link hypertext to the Internet, we need:
1.	The markup language, i.e., HTML.
2.	The transfer protocol, e.g., HTTP.
3.	Uniform Resource Locator (URL), the address of the resource.

We access the web using web browsers.

URI (Uniform Resource Identifier) - it’s like an address providing a unique global identifier to a resource on the Web. Uniform Resource Locator (URL) is the most commonly used form of a URI.

The URL consists mainly of two parts:
1.	The protocol used in the transfer, e.g., HTTP.
2.	The domain name.

## AWS VPC (7.07 thru 7.11)

Amazon Virtual Private Cloud (Amazon VPC) lets you provision a logically isolated section of the AWS Cloud where you can launch AWS resources in a virtual network that you define. You have complete control over your virtual networking environment, including selection of your own IP address range, creation of subnets, and configuration of route tables and network gateways. You can use both IPv4 and IPv6 in your VPC for secure and easy access to resources and applications.

This enables you to provision logically isolated sections of the AWS Cloud where you can launch AWS resources in your virtual network. You have control over your virtual networking resources including:
  * Selection of IP address ranges
  * Creation of Subnets
  * Configuration of route tables and network gateways

## VPC Networking (7.12 thru 7.19)

Internet gateway - is a horizontally scaled, redundant, and highly available VPC component that allows communication between your VPC and the internet. An internet gateway serves two purposes: to provide a target in your VPC route tables for internet-routable traffic, and to perform network address translation (NAT) for instances that have been assigned public IPv4 addresses. An internet gateway supports IPv4 and IPv6 traffic. It does not cause availability risks or bandwidth constraints on your network traffic.

Network Address Translation (NAT) device can be used to enable instances in a private subnet to connect to the internet (for example, for software updates) or other AWS services, but prevent the internet from initiating connections with the instances. A NAT device forwards traffic from the instances in the private subnet to the internet or other AWS services, and then sends the response back to the instances. When traffic goes to the internet, the source IPv4 address is replaced with the NAT device’s address and similarly, when the response traffic goes to those instances, the NAT device translates the address back to those instances’ private IPv4 addresses.

Network address translation (NAT) gateway to enable instances in a private subnet to connect to the internet or other AWS services, but prevent the internet from initiating a connection with those instances. To create a NAT gateway, you must specify the public subnet in which the NAT gateway should reside. You must also specify an Elastic IP address (Links to an external site.) to associate with the NAT gateway when you create it. The Elastic IP address cannot be changed after you associate it with the NAT Gateway. After you've created a NAT gateway, you must update the route table associated with one or more of your private subnets to point internet-bound traffic to the NAT gateway.

You can use a network address translation (NAT) instance in a public subnet in your VPC to enable instances in the private subnet to initiate outbound IPv4 traffic to the internet or other AWS services, but prevent the instances from receiving inbound traffic initiated by someone on the internet. NAT is not supported for IPv6 traffic—use an egress-only internet gateway instead.

VPC sharing allows multiple AWS accounts to create their application resources, such as Amazon EC2 instances, Amazon Relational Database Service (RDS) databases, Amazon Redshift clusters, and AWS Lambda functions, into shared, centrally-managed Amazon Virtual Private Clouds (VPCs). In this model, the account that owns the VPC (owner) shares one or more subnets with other accounts (participants) that belong to the same organization from AWS Organizations. After a subnet is shared, the participants can view, create, modify, and delete their application resources in the subnets shared with them. Participants cannot view, modify, or delete resources that belong to other participants or the VPC owner.

A VPC peering connection is a networking connection between two VPCs that enables you to route traffic between them privately. Instances in either VPC can communicate with each other as if they are within the same network. You can create a VPC peering connection between your own VPCs, with a VPC in another AWS account, or with a VPC in a different AWS Region.

VPN stands for Virtual Private Network. This technology allows a user to connect one remote private network to a seperate remote private network through a secure virtual tunnel over the public internet. Many companies use this technology to connect seperate locations in order to grant employees the ability to access company resources anywhere in the world.

AWS Direct Connect links your internal network to an AWS Direct Connect location over a standard Ethernet fiber-optic cable. One end of the cable is connected to your router, the other to an AWS Direct Connect router. With this connection, you can create virtual interfaces directly to public AWS services (for example, to Amazon S3) or to Amazon VPC, bypassing internet service providers in your network path. This private connection can reduce your network costs, increase bandwidth throughput, and provide a more consistent network experience than internet-based connections. 

A VPC endpoint enables you to privately connect your VPC to supported AWS services and VPC endpoint services powered by AWS PrivateLink without requiring an internet gateway, NAT device, VPN connection, or AWS Direct Connect connection. Instances in your VPC do not require public IP addresses to communicate with resources in the service. Traffic between your VPC and the other service does not leave the Amazon network.

Endpoints are virtual devices. They are horizontally scaled, redundant, and highly available VPC components. They allow communication between instances in your VPC and services without imposing availability risks or bandwidth constraints on your network traffic.

There are three types of VPC endpoints:
  * Endpoint service - Your own application in your VPC. Other AWS principals can create a connection from their VPC to your endpoint service 
  * Gateway endpoint - A gateway endpoint (Links to an external site.) is a gateway that you specify as a target for a route in your route table for traffic destined to a supported AWS service. 
  * Interface endpoint - An interface endpoint (Links to an external site.) is an elastic network interface with a private IP address from the IP address range of your subnet that serves as an entry point for traffic destined to a supported service.

A transit gateway is a network transit hub that you can use to interconnect your virtual private clouds (VPC) and on-premises networks. AWS Transit Gateway connects VPCs and on-premises networks through a central hub. This simplifies your network and puts an end to complex peering relationships. It acts as a cloud router – each new connection is only made once.

## VPC Security (7.20, 7.21)

A security group acts as a virtual firewall for your instance to control inbound and outbound traffic. When you launch an instance in a VPC, you can assign up to five security groups to the instance. Security groups act at the instance level, not the subnet level. Therefore, each instance in a subnet in your VPC can be assigned to a different set of security groups.

Security group basics

The following are the basic characteristics of security groups for your VPC:
  * There are quotas on the number of security groups that you can create per VPC, the number of rules that you can add to each security group, and the number of security groups that you can associate with a network interface
  * You can specify allow rules, but not deny rules.
  * You can specify separate rules for inbound and outbound traffic.
  * When you create a security group, it has no inbound rules. Therefore, no inbound traffic originating from another host to your instance is allowed until you add inbound rules to the security group.
  * By default, a security group includes an outbound rule that allows all outbound traffic. You can remove the rule and add outbound rules that allow specific outbound traffic only. If your security group has no outbound rules, no outbound traffic originating from your instance is allowed.
  * Security groups are stateful — if you send a request from your instance, the response traffic for that request is allowed to flow in regardless of inbound security group rules. Responses to allowed inbound traffic are allowed to flow out, regardless of outbound rules.
  * Instances associated with a security group can't talk to each other unless you add rules allowing the traffic (exception: the default security group has these rules by default).
  * Security groups are associated with network interfaces. After you launch an instance, you can change the security groups that are associated with the instance, which changes the security groups associated with the primary network interface (eth0). You can also specify or change the security groups associated with any other network interface. By default, when you create a network interface, it's associated with the default security group for the VPC, unless you specify a different security group.
  * When you create a security group, you must provide it with a name and a description. The following rules apply: 
    - Names and descriptions can be up to 255 characters in length.
    - Names and descriptions are limited to the following characters: a-z, A-Z, 0-9, spaces, and ._-:/()#,@[]+=&;{}!$*.
    - A security group name cannot start with sg- as these indicate a default security group.
    - A security group name must be unique within the VPC.
  * A security group can only be used in the VPC that you specify when you create the security group.

Default Security Groups

Your VPC automatically comes with a default security group. If you don't specify a different security group when you launch the instance, we associate the default security group with your instance. 

Inbound
|Destination|Protocol|Port range|Description|
|---|---|---|---|
|The security group ID (sg-xxxxxxxx)|All|All|Allow inbound traffic from network interfaces (and their associated instances) that are assigned to the same security group.|

Outbound
|Destination|Protocol|Port range|Description|
|---|---|---|---|
|0.0.0.0/0|All|All|Allow all outbound IPv4 traffic.|
|::/0|All|All|Allow all outbound IPv6 traffic. This rule is added by default if you create a VPC with an IPv6 CIDR block or if you associate an IPv6 CIDR block with your existing VPC.|

You can change the rules for the default security group, but you cannot delete it.

Custom Security Groups

When you create a custom security group, you can specify allow rules, but not deny rules. All rules are evaluated before the decision to allow traffic. The kind of rules that you add can depend on the purpose of the security group.

The following table describes example rules for a security group that's associated with web servers. The web servers can receive HTTP and HTTPS traffic from all IPv4 and IPv6 addresses, and can send SQL or MySQL traffic to a database server.

Inbound
|Destination|Protocol|Port range|Description|
|---|---|---|---|
|0.0.0.0/0|TCP|80|Allow inbound HTTP access from all IPv4 addresses|
|::/0|TCP|80|Allow inbound HTTP access from all IPv6 addresses|
|0.0.0.0/0|TCP|443|Allow inbound HTTPS access from all IPv4 addresses|
|::/0|TCP|443|Allow inbound HTTPS access from all IPv6 addresses|
|Your network's public IPv4 address range|TCP|22|Allow inbound SSH access to Linux instances from IPv4 IP addresses in your network (over the internet gateway)|
|Your network's public IPv4 address range|TCP|3389|Allow inbound RDP access to Windows instances from IPv4 IP addresses in your network (over the internet gateway)|

Outbound
|Destination|Protocol|Port range|Description|
|---|---|---|---|
|The ID of the security group for your Microsoft SQL Server database servers|TCP|1433|Allow outbound Microsoft SQL Server access to instances in the specified security group|
|The ID of the security group for your MySQL database servers|TCP|3306|Allow outbound MySQL access to instances in the specified security group|

A network access control list (ACL) is an optional layer of security for your VPC that acts as a firewall for controlling traffic in and out of one or more subnets. You might set up network ACLs with rules similar to your security groups in order to add an additional layer of security to your VPC.

Network ACL basics

The following are the basic things that you need to know about network ACLs:
  * Your VPC automatically comes with a modifiable default network ACL. By default, it allows all inbound and outbound IPv4 traffic and, if applicable, IPv6 traffic.
  * You can create a custom network ACL and associate it with a subnet. By default, each custom network ACL denies all inbound and outbound traffic until you add rules.
  * Each subnet in your VPC must be associated with a network ACL. If you don't explicitly associate a subnet with a network ACL, the subnet is automatically associated with the default network ACL.
  * You can associate a network ACL with multiple subnets. However, a subnet can be associated with only one network ACL at a time. When you associate a network ACL with a subnet, the previous association is removed.
  * A network ACL contains a numbered list of rules. We evaluate the rules in order, starting with the lowest numbered rule, to determine whether traffic is allowed in or out of any subnet associated with the network ACL. The highest number that you can use for a rule is 32766. We recommend that you start by creating rules in increments (for example, increments of 10 or 100) so that you can insert new rules where you need to later on.
  * A network ACL has separate inbound and outbound rules, and each rule can either allow or deny traffic.
  * Network ACLs are stateless, which means that responses to allowed inbound traffic are subject to the rules for outbound traffic (and vice versa).

## AWS Networking Services (7.22, 7.23)

Amazon Route 53

DNS, or the Domain Name System, translates human readable domain names (for example, www.amazon.com) to machine readable IP addresses (for example, 192.0.2.44).

All computers on the Internet, from your smart phone or laptop to the servers that serve content for massive retail websites, find and communicate with one another by using numbers. These numbers are known as IP addresses. When you open a web browser and go to a website, you don't have to remember and enter a long number. Instead, you can enter a domain name like example.com and still end up in the right place.

Amazon Route 53 is a highly available and scalable cloud Domain Name System (DNS) web service. It is designed to give developers and businesses an extremely reliable and cost effective way to route end users to Internet applications by translating names like www.example.com into the numeric IP addresses like 192.0.2.1 that computers use to connect to each other.

Amazon Route 53 enables you to improve the availability of your applications that run on AWS by:
  * Configuring backup and failover scenarios for your own applications.
  * Enabling highly available multi-Region architectures on AWS.
  * Creating health checks to monitor the health and performance of your web applications, web servers, and other resources.
  * Each health check that you create can monitor one of the following—the health of a specified resource, such as a web server; the status of other health checks; and the status of an Amazon CloudWatch alarm.

Amazon CloudFront is a fast content delivery network (CDN) service that securely delivers data, videos, applications, and APIs to customers globally with low latency, high transfer speeds, all within a developer-friendly environment. CloudFront is integrated with AWS – both physical locations that are directly connected to the AWS global infrastructure, as well as other AWS services. CloudFront works seamlessly with services including AWS Shield for DDoS mitigation, Amazon S3, Elastic Load Balancing or Amazon EC2 as origins for your applications, and Lambda@Edge to run custom code closer to customers’ users and to customize the user experience. Lastly, if you use AWS origins such as Amazon S3, Amazon EC2 or Elastic Load Balancing, you don’t pay for any data transferred between these services and CloudFront.

------

### 6. Compute (Week 2, 8, 15)

## Available Operating Systems at AWS

## AWS Compute Services + Choosing the Right Service

Cloud providers offers a wide variety of compute services allowing you to develop, deploy, run, and scale your applications and workloads in the cloud. Some of the AWS Compute services include:
  * Amazon Elastic Compute Cloud (Amazon EC2) provides resizable virtual machines.
  * Amazon EC2 Auto Scaling supports application availability by allowing you to define conditions that will automatically launch or terminate EC2 instances.
  * Amazon Elastic Container Registry (Amazon ECR) is used to store and retrieve Docker images.
  * Amazon Elastic Container Service (Amazon ECS) is a container orchestration service that supports Docker.
  * Amazon Elastic Kubernetes Service (Amazon EKS) enables you to run managed Kubernetes on AWS.
  * Amazon Lightsail provides a simple-to-use service for building an application or website.
  * AWS Batch provides a tool for running batch jobs at any scale
  * AWS Elastic Beanstalk provides a simple way to run and manage web applications.
  * AWS Fargate provides a way to run containers that reduce the need for you to manage servers or clusters.
  * AWS Lambda is a serverless compute solution. You pay only for the compute time that you use.
  * AWS Serverless Application Repository provides a way to discover, deploy, and publish serverless applications.
  * AWS Outposts provides a way to run select AWS services in your on-premises data center.
  * VMware Cloud on AWS enables you to provision a hybrid cloud without custom hardware.

Selecting compute resources that meet your requirements, performance needs, and provide great efficiency of cost and effort will enable you to accomplish more with the same number of resources. When evaluating compute options, be aware of your requirements for workload performance and cost requirements and use this to make informed decisions.

In AWS, compute is available in three forms: instances, containers, and functions:
  * Instances are virtualized servers, allowing you to change their capabilities with a button or an API call. Because resource decisions in the cloud aren’t ﬁxed, you can experiment with different server types. At AWS, these virtual server instances come in different families and sizes, and they offer a wide variety of capabilities, includ- ing solid-state drives (SSDs) and graphics processing units (GPUs).
  * Containers are a method of operating system virtualization that allow you to run an application and its dependencies in resource-isolated processes. AWS Fargate is serverless compute for containers or Amazon EC2 can be used if you need control over the installation, configuration, and management of your compute environment. You can also choose from multiple container orchestration platforms: Amazon Elastic Container Service (ECS) or Amazon Elastic Kubernetes Service (EKS).
  * Functions abstract the execution environment from the code you want to execute. For example, AWS Lambda allows you to execute code without running an instance.

Best Practices for Selecting Compute Resources:
  * Evaluate the available compute options: Understand the performance characteristics of the compute-related options available to you. Know how instances, containers, and functions work, and what advantages, or disadvantages, they bring to your workload.
  * Understand the available compute configuration options: Understand how various options complement your workload, and which configuration options are best for your system. Examples of these options include instance family, sizes, features (GPU, I/O), function sizes, container instances, and single versus multi-tenancy.
  * Collect compute-related metrics: One of the best ways to understand how your compute systems are performing is to record and track the true utilization of various resources. This data can be used to make more accurate determinations about resource requirements.
  * Determine the required configuration by right-sizing: Analyze the various performance characteristics of your workload and how these characteristics relate to memory, network, and CPU usage. Use this data to choose resources that best match your workload's profile. For example, a memory-intensive workload, such as a database, could be served best by the r-family of instances. However, a bursting workload can benefit more from an elastic container system.
  * Use the available elasticity of resources: The cloud provides the flexibility to expand or reduce your resources dynamically through a variety of mechanisms to meet changes in demand. Combined with compute-related metrics, a workload can automatically respond to changes and utilize the optimal set of resources to achieve its goal.
  * Re-evaluate compute needs based on metrics: Use system-level metrics to identify the behavior and requirements of your workload over time. Evaluate your workload's needs by comparing the available resources with these requirements and make changes to your compute environment to best match your workload's profile. For example, over time a system might be observed to be more memory-intensive than initially thought, so moving to a different instance family or size could improve both performance and efficiency.

The optimal compute service will depend on your use case. In addition to understanding the above, you should ask questions based on aspects of the project:
  * What is your application design?
  * What are your usage patterns? Consistent usage, infrequent usage?
  * Which configuration settings will you need to manage?

## Virtual Machines (inc. EC2)

Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. It is designed to make web-scale computing easier for developers.  Amazon EC2’s simple web service interface allows you to obtain and configure capacity with minimal friction. It provides you with complete control of your computing resources and lets you run on Amazon’s proven computing environment.

This allows you to build Infrastructure as a Service (IaaS) applications for instance-based virtual machines. You can provision virtual machines and manage them as you choose. This method of compute is a familiar concepts with IT professionals.

  * Amazon Elastic Compute Cloud (Amazon EC2) provides resizable compute capacity as virtual machines in the cloud.
  * Amazon EC2 Auto Scaling enables you to automatically add or remove EC2 instances according to conditions that you define.

## Containers (inc. Docker & Kubernetes)

Amazon Web Services has many different container services including Amazon Elastic Container Service, Amazon Elastic Kubernetes Service, AWS Fargate, and Amazon Elastic Container Registry. These services are instance-based and enable you to run multiple workloads on a single operating system (OS). Containers spin up more quickly than virtual machines, thus offering responsiveness. Container-based solutions continue to grow in popularity.

  * Amazon Elastic Container Service (Amazon ECS) is a highly scalable, high-performance container orchestration service that supports Docker containers.
  * Amazon Elastic Container Registry (Amazon ECR) is a fully-managed Docker container registry that makes it easy for developers to store, manage, and deploy Docker container images.
  * Amazon Elastic Kubernetes Service (Amazon EKS) makes it easy to deploy, manage, and scale containerized applications that use Kubernetes on AWS.
  * AWS Fargate is a compute engine for Amazon ECS that allows you to run containers without having to manage servers or clusters.

## Serverless (inc. AWS Lambda)

AWS Lambda lets you run code without provisioning or managing servers. You pay only for the compute time you consume—there is no charge when your code is not running.
Serverless is a category of compute where you write and deploy code, but do not manage the underlying infrastructure.It is a function based environment that is low cost where deployed code can be triggered on a schedule or events. This is a newer concept for many IT professionals but is easy to learn and use.

  * AWS Lambda enables you to run code without provisioning or managing servers. You pay only for the compute time that you consume. There is no charge when your code is not running.

## PaaS (inc. AWS Elastic Beanstalk) (Week 2 - 2.1 to 2.17 and Week 8 - 8.01 to 8.19)

As a category, platform as a service allows a company to focus on building code and applications rather than manage infrastructure. AWS Elastic Beanstalk provides a platform as a service (PaaS). It facilitates the quick deployment of applications that you create by providing all the application services that you need. AWS manages the OS, the application server, and the other infrastructure components so that you can focus on developing your application code.

  * AWS Elastic Beanstalk is a service for deploying and scaling web applications and services on familiar servers such as Apache and Microsoft Internet Information Services (IIS).

For IT professionals, it is a fast and easy service to get started, however, you loose the ability to control the underlying infrastructure.

Platform as a service (PaaS) is a complete development and deployment environment in the cloud, with resources that enable you to deliver everything from simple cloud-based apps to sophisticated, cloud-enabled enterprise applications. You purchase the resources you need from a cloud service provider on a pay-as-you-go basis and access them over a secure Internet connection.

Like IaaS, PaaS includes infrastructure—servers, storage, and networking—but also middleware, development tools, business intelligence (BI) services, database management systems, and more. PaaS is designed to support the complete web application lifecycle: building, testing, deploying, managing, and updating.

PaaS allows you to avoid the expense and complexity of buying and managing software licenses, the underlying application infrastructure and middleware or the development tools and other resources. You manage the applications and services you develop, and the cloud service provider typically manages everything else.

Common Scenarios

Organizations typically use PaaS for these scenarios:

Development framework: PaaS provides a framework that developers can build upon to develop or customize cloud-based applications. Similar to the way you create an Excel macro, PaaS lets developers create applications using built-in software components. Cloud features such as scalability, high-availability, and multi-tenant capability are included, reducing the amount of coding that developers must do.

Analytics or business intelligence: Tools provided as a service with PaaS allow organizations to analyze and mine their data, finding insights and patterns and predicting outcomes to improve forecasting, product design decisions, investment returns, and other business decisions.

Additional services: PaaS providers may offer other services that enhance applications, such as workflow, directory, security, and scheduling.

Advantages of PaaS

By delivering infrastructure as a service, PaaS offers the same advantages as IaaS. But its additional features—middleware, development tools, and other business tools—give you more advantages:

Cut coding time: PaaS development tools can cut the time it takes to code new apps with pre-coded application components built into the platform, such as workflow, directory services, security features, search, and so on.

Add development capabilities without adding staff: Platform as a Service components can give your development team new capabilities without your needing to add staff having the required skills.

Develop for multiple platforms—including mobile—more easily: Some service providers give you development options for multiple platforms, such as computers, mobile devices, and browsers making cross-platform apps quicker and easier to develop.

Use sophisticated tools affordably: A pay-as-you-go model makes it possible for individuals or organizations to use sophisticated development software and business intelligence and analytics tools that they could not afford to purchase outright.

Support geographically distributed development teams: Because the development environment is accessed over the Internet, development teams can work together on projects even when team members are in remote locations.

Efficiently manage the application lifecycle: PaaS provides all of the capabilities that you need to support the complete web application lifecycle: building, testing, deploying, managing, and updating within the same integrated environment.

------

### 7. Storage (Week 9 - 9.01 to 9.20)

Storage is basically a technology that allows a user to retain digital data onto a medium. It is one of the core components of a computer and in cloud computing, something that you need to understand the differences.

Volatile vs Non-Volatile

In a computer, there are two types of storage: Volatile and Non-Volatile.

Volatile memory is a type of storage whose contents are erased when the system's power is turned off or interrupted. For example, RAM is volatile. When you are working on a document, it is kept in RAM, and if the computer loses power, your work will be lost. For this reason, you should save your document to a file on a non-volatile storage medium, such as your hard drive.

NV or Non-volatile memory is a term used to describe any memory or storage that is saved regardless of the power to the computer is on or off. It is also called persistent storage or permanent storage. An example of non-volatile memory and storage is a computer hard drive, flash memory, and ROM. If data is stored on a hard drive, it will remain on that drive regardless if the power is interrupted, which is why it is the best place to store your data and documents. Non-volatile memory also stores your computer's time and system settings even when the power is off.

Local Storage Types

In computing, there is many forms of storage. Temporary storage, such as RAM, allows a computer to temporarily store information while the computer is in use, however when power is removed, the information stored in temporary storage is lost. Permanent storage is where you keep your operating system, applications, and other data files that you use on a computer system. The information will be saved even if there is no power to the system.

Read Only Memory (RAM) - RAM is temporary storage that allows data and programs to be stored in memory in order the operating system to use them. After the operating system has booted up, each program you open, such as the browser you're using to view this page, is loaded into memory while it is running. If too many programs are open, the computer will swap the data in the memory between the RAM and the hard disk drive.

Hard drive - can be used to store any data, including pictures, music, videos, text documents, and any files created or downloaded. Also, hard drives store files for the operating system and software programs that run on the computer. The two main types of hard drive are HDD (hard disk drive) and SSD (solid state drive).

Optical Drive - uses lasers and lights as its method of reading and writing data. The three standards of optical media are CD (compact disk), DVD (digital versatile disk or digital video disk), and Blu-ray. All standards use the same size disc, but the data is read differently for each.

Flash Drive - also referred to as a USB flash drive, data stick, pen drive, memory unit, keychain drive, and thumb drive, a jump drive is a portable storage device. It is often the size of a human thumb (hence the name) and connects to a computer via a USB port. Flash drives are an easy way to store and transfer information between computers and range in sizes from 2 GB to 1 TB.

Unlike a standard hard drive, the flash drive has no movable parts; it contains only an integrated circuit memory chip that is used to store data. Flash drives usually have plastic or aluminum casings surrounding the memory chip.

## AWS Storage Services

Storage is basically a technology that allows a user to retain digital data onto a medium. It is one of the core components of a computer and in cloud computing, something that you need to understand the differences

## S3

Amazon Simple Storage Service (Amazon S3) - is a fully managed object storage service that offers industry-leading scalability, data availability, security, and performance. This means customers of all sizes and industries can use it to store and protect any amount of data for a range of use cases, such as websites, mobile applications, backup and restore, archive, enterprise applications, IoT devices, and big data analytics. Amazon S3 provides easy-to-use management features so you can organize your data and configure finely-tuned access controls to meet your specific business, organizational, and compliance requirements. Amazon S3 is designed for 99.999999999% (11 9's) of durability, and stores data for millions of applications for companies all around the world.

Amazon S3 Features

Amazon S3 has various features you can use to organize and manage your data in ways that support specific use cases, enable cost efficiencies, enforce security, and meet compliance requirements. Data is stored as objects within resources called buckets, and a single object can be up to 5 terabytes in size. S3 features include capabilities to append metadata tags to objects, move and store data across the S3 Storage Classes, configure and enforce data access controls, secure data against unauthorized users, run big data analytics, and monitor data at the object and bucket levels. Objects can be accessed through S3 Access Points or directly through the bucket hostname.

When you create a bucket in Amazon S3, it is associated with a specific AWS Region. When you store data in the bucket, it is redundantly stored across multiple AWS facilities within your selected Region. Amazon S3 is designed to durably store your data, even if there is concurrent data loss in two AWS facilities.
Amazon S3 automatically manages the storage behind your bucket while your data grows. You can get started immediately, and your data storage will grow with your application needs. Amazon S3 also scales to handle a high volume of requests. You do not need to provision the storage or throughput, and you are billed only for what you use.

## Glacier

Amazon S3 Glacier - is a secure, durable, and extremely low-cost storage service for data archiving and long-term backup. It is designed to deliver 99.999999999% durability, and provides comprehensive security and compliance capabilities that can help meet even the most stringent regulatory requirements. Amazon S3 Glacier provides query-in-place functionality, allowing you to run powerful analytics directly on your archive data at rest. You can store data for as little as $0.004 per gigabyte per month, a significant savings compared to on-premises solutions. To keep costs low yet suitable for varying retrieval needs, Amazon S3 Glacier provides three options for access to archives, from a few minutes to several hours

Glacier Features & Terms

Amazon S3 Glacier is a data archiving service that is designed for security, durability, and an extremely low cost.
  * Amazon S3 Glacier is designed to provide 11 9s of durability for objects.
  * It supports the encryption of data in transit and at rest through Secure Sockets Layer (SSL) or Transport Layer Security (TLS).
  * The Vault Lock feature enforces compliance through a policy.

When you use Amazon S3 Glacier to archive data, you can store your data at an extremely low cost (even in comparison to Amazon S3), but you cannot retrieve your data immediately when you want it. Data that is stored in Amazon S3 Glacier can take several hours to retrieve, which is why it works well for archiving.

There are three key Amazon S3 Glacier terms you should be familiar with:
  * Archive – Any object (such as a photo, video, file, or document) that you store in Amazon S3 Glacier. It is the base unit of storage in Amazon S3 Glacier. Each archive has its own unique ID and it can also have a description.
  * Vault – A container for storing archives. When you create a vault, you specify the vault name and the Region where you want to locate the vault.
  * Vault access policy – Determine who can and cannot access the data that is stored in the vault, and what operations users can and cannot perform. One vault access permissions policy can be created for each vault to manage access permissions for that vault. You can also use a vault lock policy to make sure that a vault cannot be altered. Each vault can have one vault access policy and one vault lock policy that are attached to it.

Amazon S3 Glacier provides three options for access to archives—expedited, standard, and bulk—retrieval times range from a few minutes to several hours.
  * Expedited retrievals are typically made available within 1–5 minutes (highest cost).
  * Standard retrievals typically complete within 3–5 hours (less time than expedited, more time than bulk).
  * Bulk retrievals typically complete within 5–12 hours (lowest cost).

You might compare these options to choosing the cost for shipping a package by using the most economical method for your needs

## EBS

Amazon Elastic Block Store (Amazon EBS) - provides persistent block storage volumes for use with Amazon EC2 instances in the AWS Cloud. Each Amazon EBS volume is automatically replicated within its Availability Zone to protect you from component failure, offering high availability and durability. Amazon EBS volumes offer the consistent and low-latency performance needed to run your workloads. With Amazon EBS, you can scale your usage up or down within minutes—all while paying a low price for only what you provision.

Amazon EBS allows you to create storage volumes and attach them to Amazon EC2 instances. Once attached, you can create a file system on top of these volumes, run a database, or use them in any other way you would use block storage. Amazon EBS volumes are placed in a specific Availability Zone where they are automatically replicated to protect you from the failure of a single component. All EBS volume types offer durablesnapshot capabilities to S3 and are designed for 99.999% availability.

EBS Features

Snapshots

Amazon EBS provides the ability to save point-in-time snapshots of your volumes to Amazon S3. Amazon EBS Snapshots are stored incrementally: only the blocks that have changed after your last snapshot are saved, and you are billed only for the changed blocks. If you have a device with 100 GB of data but only 5 GB has changed after your last snapshot, a subsequent snapshot consumes only 5 additional GB and you are billed only for the additional 5 GB of snapshot storage, even though both the earlier and later snapshots appear complete.

Encryption

Amazon EBS encryption offers seamless encryption of EBS data volumes, boot volumes and snapshots, eliminating the need to build and manage a secure key management infrastructure. EBS encryption enables data at rest security by encrypting your data volumes, boot volumes and snapshots using Amazon-managed keys or keys you create and manage using the AWS Key Management Service (KMS). In addition, the encryption occurs on the servers that host EC2 instances, providing encryption of data as it moves between EC2 instances and EBS data and boot volumes.

Elasticity

Elastic Volumes is a feature that allows you to easily adapt your volumes as the needs of your applications change. Elastic Volumes allows you to dynamically increase capacity, tune performance, and change the type of any new or existing current generation volume with no downtime or performance impact. Easily right-size your deployment and adapt to performance changes.

## EFS

Amazon Elastic File System (Amazon EFS) - provides a simple, scalable, elastic file system for Linux-based workloads for use with AWS Cloud services and on-premises resources. It is built to scale on demand to petabytes without disrupting applications, growing and shrinking automatically as you add and remove files, so your applications have the storage they need – when they need it. It is designed to provide massively parallel shared access to thousands of Amazon EC2 instances, enabling your applications to achieve high levels of aggregate throughput and IOPS with consistent low latencies. Amazon EFS is a fully managed service that requires no changes to your existing applications and tools, providing access through a standard file system interface for seamless integration. Amazon EFS is a regional service storing data within and across multiple Availability Zones (AZs) for high availability and durability. You can access your file systems across AZs and regions and share files between thousands of Amazon EC2 instances and on-premises servers via AWS Direct Connect or AWS VPN.

Amazon EFS is well suited to support a broad spectrum of use cases from highly parallelized, scale-out workloads that require the highest possible throughput to single-threaded, latency-sensitive workloads. Use cases such as lift-and-shift enterprise applications, big data analytics, web serving and content management, application development and testing, media and entertainment workflows, database backups, and container storage.

Amazon EFS Features

Amazon Elastic File System (Amazon EFS) provides a simple, scalable, fully managed, elastic NFS file system. It is built to scale on demand to petabytes without disrupting applications, growing and shrinking automatically as you add and remove files, eliminating the need to provision and manage capacity to accommodate growth.

Features Include:
  * File storage in the AWS Cloud
  * Works well for big data and analytics, media processing workflows, content management, web serving, and home directories
  * Petabyte-scale, low-latency file system
  * Shared Storage
  * Elastic Capacity
  * Supports Network File System (NFS) versions 4.0 and 4.1 (NFSv4)
  * Compatible with all Linux-based AMIs for Amazon EC2

------

### 8. Databases (Week 10 - 10.01 to 10.12)

A database is a shared collection of related data used to support the activities of a particular organization. A database can be viewed as a repository of data that is defined once and then accessed by various users.

A database has the following properties:
  * It is a representation of some aspect of the real world or a collection of data elements (facts) representing real-world information.
  * A database is logical, coherent and internally consistent.
  * A database is designed, built and populated with data for a specific purpose.
  * Each data item is stored in a field.
  * A combination of fields makes up a table. For example, each field in an employee table contains data about an individual employee.

The SQL data manipulation language (DML) is used to query and modify database data. SQL DML command statements, defined below.
  * SELECT – to query data in the database
  * INSERT – to insert data into a table
  * UPDATE – to update data in a table
  * DELETE – to delete data from a table

Relational DBs (SQL based)

This DB consists of a collection of tables (like CSV tables), that are connected. Each row in a table represents a record.

Why is it called relational? What are the ‘relations’ that exist in this DB?

Let ’s say you have a table of students information, and a table of the course grades (course, grade, student id), every grade row relates to a student record.

All relational DBs are queried with SQL-like languages, which are commonly used and inherently support join operations. They allow the indexing of columns for faster queries based on those columns. Because of its structured nature, the relational DB’s schema is decided before inserting data.

Common relational databases: MySQL, PostgreSQL, Oracle, MS SQL Server

NoSQL DBs

While in relational DBs everything is structured to rows and columns, in NoSQL DBs there is no common structured schema for all records. Most of the NoSQL databases contain JSON records, and different records can include different fields.

This family of databases should actually be called “Not mainly SQL” — since many NoSQL DBs support querying using SQL, but using it is not the best practice for them.

There are 4 main types of NoSQL databases:
1. Document-oriented DBs

The atomic unit of this DB is a document.

Each document is a JSON, the schema can vary between different documents and contain different fields.

Document DBs allow indexing of some fields in the document to allow faster queries based on those fields (this forces all the documents to have the field).

When should I use it?
Data analysis — Since different records are not dependent on one another (logic and structure-wise) this DB supports parallel computations.
This allows you to perform big data analytics on our data easily.
Common document-based databases: MongoDB, CouchDB, DocumentDB.

2. Columnar DBs

The atomic unit of this DB is a column in the table, meaning the data is stored column by column. It makes column-based queries very efficient, and since the data on each column is quite homogeneous, this allows better compression of the data.

When should I use it?

When you tend to query on a subset of columns in your data (doesn’t need to be the same subset each time!).

Columnar DB performs such queries very fast since it only needs to read these specific columns (while row-based DB would have to read the entire data).
  * This is often common in data science, where each column represents a feature. As a data scientist, I often train my models with subsets of the features and tend to check relations between features and scores (correlation, variance, significance).
  * This is also common with logs — we often store a lot more fields in our logs database but uses only a few in each query.

Common column DB database: Cassandra.

3. Key-value DBs

The querying is only key-based — You ask for a key and get its value.

Doesn’t support queries across different record values like ‘select all records where city == New York’

A useful feature in this DB is the TTL field (time to live), this field can be set differently for each record and state when it should be deleted from the DB.

Advantages — It is very fast.

First because of the use of unique keys, and second because most of the key-values databases store the data in memory (RAM) which allows quick access.
Disadvantages — You need to define unique keys that are good identifiers and built of the data you know in the time of the query.
Often more expensive than other kinds of databases (since runs on memory).

When should I use it?

Mainly used for cache since it is very fast and doesn’t require complex querying, also the TTL feature comes very useful for caching. It can also be used for any other kind of data that requires fast querying and meets the key-value format.

Common key-value databases: Redis, Memcached

4. Graph DBs

Graph DBs contain nodes that represent entities and edges that represent relationships between entities.

When should I use it?

When your data is a graph like, like knowledge graphs and social networks.

Common graph databases: Neo4j, InfiniteGraph

## AWS Databases

## AWS Relational Database Services

Amazon RDS is a managed relational database service that provides you six familiar database engines to choose from, including Amazon Aurora , MySQL , MariaDB , Oracle , Microsoft SQL Server , and PostgreSQL . This means that the code, applications, and tools you already use today with your existing databases can be used with Amazon RDS. Amazon RDS handles routine database tasks such as provisioning, patching, backup, recovery, failure detection, and repair.

Amazon RDS makes it easy to use replication to enhance availability and reliability for production workloads. Using the Multi-AZ (Links to an external site.) deployment option, you can run mission-critical workloads with high availability and built-in automated fail-over from your primary database to a synchronously replicated secondary database. Using Read Replicas, you can scale out beyond the capacity of a single database deployment for read-heavy database workloads.

As with all Amazon Web Services, there are no up-front investments required, and you pay only for the resources you use.

When to Choose Amazon RDS

Use Amazon RDS when your application requires:
  * Complex transactions or complex queries
  * A medium to high query or write rate – up to 30,000 IOPS (15,000 reads + 15,000 writes)
  * No more than a single worker node or shard
  * High durability

Do not use Amazon RDS when your application requires:
  * Massive read/write rates (for example 150,000 writes per second)
  * Sharding due to high data size or throughput demands
  * Simple GET or PUT requests and queries that a NoSQL database can handle
  * Or, relational database management system (RDBMS) customization

For circumstances when you should not use Amazon RDS, consider either using a NoSQL database solution (such as DynamoDB) or running your relational database engine on Amazon EC2 instances instead of Amazon RDS (which will provide you with more options for customizing your database).

## AWS Dynamo DB

Amazon DynamoDB is a fully managed key-value and document NoSQL database service that provides fast and predictable performance with seamless scalability. DynamoDB lets you offload the administrative burdens of operating and scaling a distributed database so that you don't have to worry about hardware provisioning, setup and configuration, replication, software patching, or cluster scaling. DynamoDB also offers encryption at rest, which eliminates the operational burden and complexity involved in protecting sensitive data.

Amazon manages all the underlying data infrastructure for this service and redundantly stores data across multiple facilities in a native US Region as part of the fault-tolerant architecture. With DynamoDB, you can create tables and items. You can add items to a table. The system automatically partitions your data and has table storage to meet workload requirements. There is no practical limit on the number of items that you can store in a table. For instance, some customers have production tables that contain billions of items.

As your application becomes more popular and as users continue to interact with it, your storage can grow with your application's needs. All the data in DynamoDB is stored on solid state drives (SSDs) and its simple query language enables consistent low-latency query performance. In addition to scaling storage, DynamoDB also enables you to provision the amount of read or write throughput that you need for your table. As the number of application users grows, DynamoDB tables can be scaled to handle the increased numbers of read/write requests with manual provisioning. Alternatively, you can enable automatic scaling so that DynamoDB monitors the load on the table and automatically increases or decreases the provisioned throughput.

Some additional key features include global tables that enable you to automatically replicate across your choice of AWS Regions, encryption at rest, and item Time-to-Live (TTL)

Core Components

Tables, Items, and Attributes

Key Features:
  * NoSQL database tables
  * Virtually unlimited storage
  * Items can have differing attributes
  * Low-latency queries
  * Scalable read/write throughput

The following are the basic DynamoDB components:
  * Tables – Similar to other database systems, DynamoDB stores data in tables. A table is a collection of data. For example, see the example table called People that you could use to store personal contact information about friends, family, or anyone else of interest. You could also have a Cars table to store information about vehicles that people drive.
  * Items – Each table contains zero or more items. An item is a group of attributes that is uniquely identifiable among all of the other items. In a People table, each item represents a person. For a Cars table, each item represents one vehicle. Items in DynamoDB are similar in many ways to rows, records, or tuples in other database systems. In DynamoDB, there is no limit to the number of items you can store in a table.
  * Attributes – Each item is composed of one or more attributes. An attribute is a fundamental data element, something that does not need to be broken down any further. For example, an item in a People table contains attributes called PersonID, LastName, FirstName, and so on. For a Department table, an item might have attributes such as DepartmentID, Name, Manager, and so on. Attributes in DynamoDB are similar in many ways to fields or columns in other database systems.

Primary Key

When you create a table, in addition to the table name, you must specify the primary key of the table. The primary key uniquely identifies each item in the table, so that no two items can have the same key.
  * Partition key – A simple primary key, composed of one attribute known as the partition key.
  * Partition key and sort key – Referred to as a composite primary key, this type of key is composed of two attributes. The first attribute is the partition key, and the second attribute is the sort key.

Secondary Indexes

You can create one or more secondary indexes on a table. A secondary index lets you query the data in the table using an alternate key, in addition to queries against the primary key. DynamoDB doesn't require that you use indexes, but they give your applications more flexibility when querying your data. After you create a secondary index on a table, you can read data from the index in much the same way as you do from the table.
DynamoDB supports two kinds of indexes:
  * Global secondary index – An index with a partition key and sort key that can be different from those on the table.
  * Local secondary index – An index that has the same partition key as the table, but a different sort key.

## AWS Redshift

Amazon Redshift is a fully managed, petabyte-scale data warehouse service in the cloud. You can start with just a few hundred gigabytes of data and scale to a petabyte or more. This enables you to use your data to acquire new insights and analytics for your business and customers.

Redshift is integrated with data lakes which are usually a single store of all enterprise data including raw copies of source system data and transformed data used for tasks such as reporting, visualization, advanced analytics and machine learning. It offers up to 3x faster performance than any other data warehouse, and costs up to 75% less than any other cloud data warehouse.

It simple and cost-effective to analyze all your data by using standard SQL and your existing business intelligence (BI) tools. It enables you to run complex analytic queries against petabytes of structured data by using sophisticated query optimization, columnar storage on high-performance local disks, and massively parallel query execution. Most results come back in seconds

How does it work?

An Amazon Redshift cluster consists of nodes. Each cluster has a leader node and one or more compute nodes. The leader node receives queries from client applications, parses the queries, and develops query execution plans. The leader node then coordinates the parallel execution of these plans with the compute nodes and aggregates the intermediate results from these nodes. It then finally returns the results back to the client applications.
Compute nodes execute the query execution plans and transmit data among themselves to serve these queries. The intermediate results are sent to the leader node for aggregation before being sent back to the client applications.

Automation & Scaling
  * It is straightforward to automate most of the common administrative tasks to manage, monitor, and scale your Amazon Redshift cluster—which enables you to focus on your data and your business.
  * Scalability is intrinsic in Amazon Redshift. Your cluster can be scaled up and down as your needs change with a few clicks in the console.
  * Security is the highest priority for AWS. With Amazon Redshift, security is built in, and it is designed to provide strong encryption of your data both at rest and in transit.

## AWS Aurora

Amazon Aurora is a MySQL and PostgreSQL-compatible relational database built for the cloud, that combines the performance and availability of traditional enterprise databases with the simplicity and cost-effectiveness of open source databases. Using Amazon Aurora can reduce your database costs while improving the reliability and availability of the database. As a fully managed service, Aurora is designed to automate time-consuming tasks like provisioning, patching, backup, recovery, failure detection, and repair.

Amazon Aurora is designed to be highly available: it stores multiple copies of your data across multiple Availability Zones with continuous backups to Amazon S3. Amazon Aurora can use up to 15 read replicas can be used to reduce the possibility of losing your data. Additionally, Amazon Aurora is designed for instant crash recovery if your primary database becomes unhealthy.

After a database crash, Amazon Aurora does not need to replay the redo log from the last database checkpoint. Instead, it performs this on every read operation. This reduces the restart time after a database crash to less than 60 seconds in most cases.

------

### 9. Cloud Architecture (Week 11 - 11.01-11.05)

## Document: AWS Well Architected Framework

The AWS Well-Architected Framework helps you understand the pros and cons of decisions you make while building systems on AWS. By using the Framework you will learn architectural best practices for designing and operating reliable, secure, efficient, and cost-effective systems in the cloud.

## Reliability

One of the best practices that is identified in the AWS Well-Architected Framework is to plan for failure (or application or workload downtime). One way to do that is to architect your applications and workloads to withstand failure. There are two important factors that cloud architects consider when designing architectures to withstand failure: reliability and availability.

Reliability - is the measure of your systems ability to perform its intended function correctly and consistently when it’s expected to. This means the system is available for use and able to operate the workload through its total lifecycle. All apects of the system must be considered including: hardware, firmware and software. Failure of any one of these impacts the reliabilty of the system.

Reliability should be considered a statistical tool. No system is perfect and there is always the probability that your system will function as intended for a specified period of time.

Should a failure happen, this will affect the "mean time between failures" (MTBF) is equal to the total time in service divided by the number of failures.
For example, think about a car as a system. It contains an engine, brakes, ignition, and much more. All of the components must work for the entire system to work. If the ignition fails, the car cannot be started and the system has failed. If this has happened only once in the time you own the car, the MTBF is very low and the car is reliable, but if it happens every month, the MTBF is very high and the car is not reliable.

Another metric is the mean time to failure (MTTF) which is the length of time a system is available until it fails. Once it does fail, you need to repair and bring the system back online. The mean time to repair (MTTR) is the amount of time taken to repair a system. The MTBF can be expanded to equal MTTF + MTTR divided by the number of failures.

This creates a failure-repair-restore cycle that:
1.	A system is brought online and is available
2.	A system component then fails, we can now calculate the MTBF
3.	A system component is repaired, we can now calculate the MTTR
4.	A system is brought back online after repair, we can now calculate the MTBF

## Availability

Availability - is used to describe the period of time when a service is available, as well as the time required by a system to respond to a request made by a user. Availability (AKA service availability) is a commonly used metric to quantitatively measure reliability. Availability is defined as the percentage of time that a workload is available for use. Available for use means that it performs its agreed function when required.

Availability = "Available for Use Time" / "Total Time"

This number the percentage of up-time over a period of a time, normally a year. Common short-hand refers only to the "number of 9's"; for example, "five nines" translates to being 99.999% available.

Factors that influence availability include:
  * Fault Tolerance: built in redundancy of a system or application so it can remain operational
  * Scalability: ability to accommodate increase or decrease in capacity usage without changing the design
  * Recoverability: process, policies, and procedures related to restoring a system after system failure

High availability (HA) is a quality of a system or component that assures a high level of operational performance for a given period of time. A system can degrade, but still remain available in a HA system. Therefore downtime and required human intervention are minimized.

High availability functions as a failure response mechanism for infrastructure. The way that it works is quite simple conceptually but typically requires some specialized software and configuration.

Implementing high availability for your infrastructure is a useful strategy to reduce the impact of these types of events. Highly available systems can recover from server or component failure automatically.

Availablity Tiers
|Availability|Maximum Unavailability (per year)|Application Categories|
|---|---|---|
|99%|3 days 15 hours|Batch processing, data extraction, transfer, and load jobs|
|99.9%|8 hours 45 minutes|Internal tools like knowledge management, project tracking|
|99.95%|4 hours 22 minutes|Online commerce, point of sale|
|99.99%|52 minutes|Video delivery, broadcast workloads|
|99.999%|5 minutes|ATM transactions, telecommunications workloads|

## AWS Trusted Advisor

The AWS Well-Architected Tool (AWS WA Tool) helps you review the state of your workloads and compares them to the latest AWS architectural best practices. The tool is based on the AWS Well-Architected Framework (Links to an external site.), developed to help cloud architects build secure, high-performing, resilient, and efficient application infrastructure. This Framework provides a consistent approach for customers and partners to evaluate architectures, has been used in tens of thousands of workload reviews conducted by the AWS solutions architecture team, and provides guidance to help implement designs that scale with application needs over time.

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

### 10. Automatic Scaling & Monitoring

## AWS CloudWatch

## Amazon EC2 AutoScaling

## Chapter 5 via O'Reilly: Planning for Scale & Resiliency

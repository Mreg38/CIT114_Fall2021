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

## PaaS (inc. AWS Elastic Beanstalk) (Week 2 - 2.1 to 2.17)

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

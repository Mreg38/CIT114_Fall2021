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

## AWS Perspective

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

## Software as a Service (SaaS)

Software as a service (SaaS) allows users to connect to and use cloud-based apps over the Internet. Common examples are email, calendaring, and office tools (such as Microsoft Office 365).

SaaS provides a complete software solution that you purchase on a pay-as-you-go basis from a cloud service provider.  You rent the use of an app for your organization, and your users connect to it over the Internet, usually with a web browser. All of the underlying infrastructure, middleware, app software, and app data are located in the service provider’s data center. The service provider manages the hardware and software, and with the appropriate service agreement, will ensure the availability and the security of the app and your data as well. SaaS allows your organization to get quickly up and running with an app at minimal upfront cost.

Common Scenarios

If you’ve used a web-based email service such as Outlook, Hotmail, or Yahoo! Mail, then you’ve already used a form of SaaS. With these services, you log into your account over the Internet, often from a web browser. The email software is located on the service provider’s network, and your messages are stored there as well. You can access your email and stored messages from a web browser on any computer or Internet-connected device.

The previous examples are free services for personal use. For organizational use, you can rent productivity apps, such as email, collaboration, and calendaring; and sophisticated business applications such as customer relationship management (CRM), enterprise resource planning (ERP), and document management. You pay for the use of these apps by subscription or according to the level of use.

Advantages of SaaS

Gain access to sophisticated applications: To provide SaaS apps to users, you don’t need to purchase, install, update, or maintain any hardware, middleware, or software. SaaS makes even sophisticated enterprise applications, such as ERP and CRM, affordable for organizations that lack the resources to buy, deploy, and manage the required infrastructure and software themselves.

Pay only for what you use: You also save money because the SaaS service automatically scales up and down according to the level of usage.
Use free client software. Users can run most SaaS apps directly from their web browser without needing to download and install any software, although some apps require plugins. This means that you don’t need to purchase and install special software for your users.

Mobilize your workforce easily: SaaS makes it easy to “mobilize” your workforce because users can access SaaS apps and data from any Internet-connected computer or mobile device. You don’t need to worry about developing apps to run on different types of computers and devices because the service provider has already done so. In addition, you don’t need to bring special expertise onboard to manage the security issues inherent in mobile computing. A carefully chosen service provider will ensure the security of your data, regardless of the type of device consuming it.

Access app data from anywhere: With data stored in the cloud, users can access their information from any Internet-connected computer or mobile device. And when app data is stored in the cloud, no data is lost if a user’s computer or device fails.

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

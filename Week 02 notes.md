# CIT 114 Week 2 (Notes 03: Cloud Global Infrastructure)
## Here are some important thinkgs I learned in Week 2
### Introducing Cloud Computing/Cloud Global Infrastructure

#### A Brief History
The idea of computing in a "cloud" traces back to the origins of utility computing, a concept that computer scientist John McCarthy publicly proposed in 1961:

If computers of the kind I have advocated become the computers of the future, then computing may someday be organized as a public utility just as the telephone
system is a public utility... The computer utility could become the basis of a new and important industry.

#### Business Drivers
Capacity planning:
The process of determining and fulfilling future demands of an organization's IT resources, products, and services.

Different capacity planning strategies exist:
  * Lead Strategy - adding capacity to an IT resource in anticipation of demand
  * Lag Strategy - adding capacity when the IT resource reaches its full capacity
  * Match Strategy - adding IT resource capacity in small increments, as demand increases

Cost Reduction:
Two costs need to be accounted for: the cost of acquiring new infrastructure, and the cost of its ongoing ownership. Operational overhead represents a considerable share of IT budgets, often exceeding up-front investment costs.

Common forms of infrastructure-related operating overhead include the following:
  * technical personnel required to keep the environment operational
  * upgrades and patches that introduce additional testing and deployment cycles
  * utility bills and capital expense investments for power and cooling
  * security and access control measures that need to be maintained and enforced to protect infrastructure resources
  * administrative and accounts staff that may be required to keep track of licenses and support arrangements

Organizational Agility:
The measure of an organization's responsiveness to change.

#### Concepts and Terminology
Cloud - refers to a distinct IT environment that is designed for the purpose of remotely provisioning scalable and measured IT resources

IT resource - a physical or virtual IT-related artifact that can be either software based, such as a virtual server or a custom software program, or hardware-based, such as a physical server or a network device

On-Premise - a way of stating "on the premises of a controlled IT environment that is not cloud-based." This term is used to qualify an IT resource as an alternative to "cloud-based." An IT resource that is on-premise cannot be cloud-based, and vice-versa.

Scaling - the ability of the IT resource to handle increased or decreased usage demands.

The following are types of scaling:
  * Horizontal Scaling - scaling out and scaling in (allocating or releasing of IT resources that are of the same type is referred to as horizontal scaling)
  * Vertical Scaling - scaling up and scaling down (existing IT resource is replaced by another with higher or lower capacity, vertical scaling)

Cloud Service - is any IT resource that is made remotely accessible via a cloud. Unlike other IT fields that fall under the service technology umbrella - such as service-oriented architecture - the term "service" within the context of cloud computing is especially broad

Cloud service consumer - a temporary runtime role assumed by a software program when it accesses a cloud service.

#### Goals and Benefits

Reduced Investments and Proportional Costs

Common measurable beneﬁts to cloud consumers include:
  * On-demand access to pay-as-you-go computing resources on a short-term basis (such as processors by the hour), and the ability to release these computing resources when they are no longer needed.
  * The perception of having unlimited computing resources that are available on demand, thereby reducing the need to prepare for provisioning.
  * The ability to add or remove IT resources at a ﬁne-grained level, such as modifying available storage disk space by single gigabyte increments.
  * Abstraction of the infrastructure so applications are not locked into devices or locations and can be easily moved if needed.

Increased Scalability

By providing pools of IT resources, along with tools and technologies designed to leverage them collectively, clouds can instantly and dynamically allocate IT resources to cloud consumers, on-demand or via the cloud consumer's direct conﬁguration.

Increased Availability and Reliability

A hallmark of the typical cloud environment is its intrinsic ability to provide extensive support for increasing the availability of a cloud-based IT resource to minimize or even eliminate outages, and for increasing its reliability so as to minimize the impact of runtime failure conditions.
Specifically:
  * An IT resource with increased availability is accessible for longer periods of time (for example, 22 hours out of a 24 hour day). Cloud providers generally offer "resilient" IT resources for which they are able to guarantee high levels of availability.
  * An IT resource with increased reliability is able to better avoid and recover from exception conditions. The modular architecture of cloud environments provides extensive failover support that increases reliability.

#### From Google's Perspective

1. Cloud computing is user-centric
2. Cloud computing is task-centric
3. Cloud computing is powerful
4. Cloud computing is accessible
5. Cloud computing is intelligent
6. Cloud computing is programmable

#### Infrastructure as a Service (IaaS)

Infrastructure as a service (IaaS) is an instant computing infrastructure, provisioned and managed over the Internet. Quickly scale up and down with demand, and pay only for what you use.

Common Scenarios:
  * Test and development
  * Website hosting
  * Storage, backup, and recovery
  * Web apps
  * High-performance computing
  * Big data analysis

Advantages of IAAS:
  * Eliminates capital expense and reduces ongoing cost
  * Improves business continuity and disaster recovery
  * Innovate rapidly
  * Respond quicker to shifting business conditions
  * Focus on your core business
  * Increase stability, reliability, and supportability
  * Better security
  * Gets new apps to users faster

Infrastructure as a Service (IaaS) contains the basic building blocks for cloud IT and typically provides access to networking features, computers (virtual or on dedicated hardware), and data storage space. IaaS provides you with the highest level of flexibility and management control over your IT resources and is most similar to existing IT resources that many IT departments and developers are familiar with today.

IaaS User/Enterprise Maintained:
  * Application
  * Data
  * Runtime
  * Middleware
  * Operating System

IaaS Provider Maintained:
  * Virtualization
  * Networking
  * Storage
  * Servers

#### Platform as a Service (PaaS)

Platform as a service (PaaS) is a complete development and deployment environment in the cloud, with resources that enable you to deliver everything from simple cloud-based apps to sophisticated, cloud-enabled enterprise applications

Common Scenarios:
  * Development framework
  * Analytics or business intelligence
  * Additional services

Advantages of PaaS:

By delivering infrastructure as a service, PaaS offers the same advantages as IaaS. But its additional features—middleware, development tools, and other business tools—give you more advantages:
  * Cut coding time
  * Add development capabilities without adding staff
  * Develop for multiple platforms—including mobile—more easily
  * Use sophisticated tools affordably
  * Support geographically distributed development teams
  * Efficiently manage the application lifecycle

Platform as a Service (PaaS) removes the need for your organization to manage the underlying infrastructure (usually hardware and operating systems) and allows you to focus on the deployment and management of your applications. This helps you be more efficient as you don’t need to worry about resource procurement, capacity planning, software maintenance, patching, or any of the other undifferentiated heavy lifting involved in running your application.

PaaS User/Enterprise Maintained:
  * Application
  * Data
PaaS Provider Maintained:
  * Runtime
  * Middleware
  * Operating System
  * Virtualization
  * Networking
  * Storage
  * Servers

#### Software as a Service (SaaS)

Software as a service (SaaS) allows users to connect to and use cloud-based apps over the Internet. Common examples are email, calendaring, and office tools (such as Microsoft Office 365).

Common Scenarios:
Web-based email service such as Outlook, Hotmail, or Yahoo! Mail. With these services, you log into your account over the Internet, often from a web browser. The email software is located on the service provider’s network, and your messages are stored there as well. You can access your email and stored messages from a web browser on any computer or Internet-connected device.

Advantages of SaaS:
  * Gain access to sophisticated applications
  * Pay only for what you use
  * Use free client software
  * Mobilize your workforce easily
  * Access app data from anywhere

Software as a Service (SaaS) provides you with a completed product that is run and managed by the service provider. In most cases, people referring to Software as a Service are referring to end-user applications. With a SaaS offering you do not have to think about how the service is maintained or how the underlying infrastructure is managed; you only need to think about how you will use that particular piece of software. A common example of a SaaS application is web-based email which you can use to send and receive email without having to manage feature additions to the email product or maintain the servers and operating systems that the email program is running on.

SaaS Provider Maintained:
  * Application
  * Data
  * Runtime
  * Middleware
  * Operating System
  * Virtualization
  * Networking
  * Storage
  * Servers

#### Cloud Computing Deployment Models

Cloud - A cloud-based application is fully deployed in the cloud and all parts of the application run in the cloud. Applications in the cloud have either been created in the cloud or have been migrated from an existing infrastructure to take advantage of the benefits of cloud computing.

Hybrid - A hybrid deployment is a way to connect infrastructure and applications between cloud-based resources and existing resources that are not located in the cloud. The most common method of hybrid deployment is between the cloud and existing on-premises infrastructure to extend, and grow, an organization's infrastructure into the cloud while connecting cloud resources to the internal system.

On-premises - The deployment of resources on-premises, using virtualization and resource management tools, is sometimes called the “private cloud.” On-premises deployment doesn’t provide many of the benefits of cloud computing but is sometimes sought for its ability to provide dedicated resources.





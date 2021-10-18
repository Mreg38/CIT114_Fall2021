# CIT 114 Week 8
## Here are some important thinkgs I learned in Week 8
### Notes 06: Compute

#### What is an Operating System

An operating system is the most important software that runs on a computer. It manages the computer's memory and processes, as well as all of its software and hardware. It also allows you to communicate with the computer without knowing how to speak the computer's language. Without an operating system, a computer is useless.

Operating system (OS) manages all of the software and hardware on the computer. Most of the time, there are several different computer programs running at the same time, and they all need to access your computer's central processing unit (CPU), memory, and storage. The operating system coordinates all of this to make sure each program gets what it needs.

Operating systems usually come pre-loaded on any computer you buy. Most people use the operating system that comes with their computer, but it's possible to upgrade or even change operating systems. The three most common operating systems for personal computers are Microsoft Windows, macOS, and Linux.

Modern operating systems use a graphical user interface, or GUI (pronounced gooey). A GUI lets you use your mouse to click icons, buttons, and menus, and everything is clearly displayed on the screen using a combination of graphics and text.

Microsoft created the Windows operating system in the mid-1980s. There have been many different versions of Windows, but the most recent ones are Windows 10 (released in 2015), Windows 8 (2012), Windows 7 (2009), and Windows Vista (2007). Windows comes pre-loaded on most new PCs, which helps to make it the most popular operating system in the world.

Linux (pronounced LINN-ux) is a family of open-source operating systems, which means they can be modified and distributed by anyone around the world. This is different from proprietary software like Windows, which can only be modified by the company that owns it. The advantages of Linux are that it is free, and there are many different distributions (or versions) you can choose from.

#### AWS Compute Services

In Amazon Web Services, there are four broad categories of compute services. These are:
  * Virtual Machines
Amazon Elastic Compute Cloud (Amazon EC2) - a web service that provides secure, resizable compute capacity in the cloud. It is designed to make web-scale computing easier for developers.  Amazon EC2’s simple web service interface allows you to obtain and configure capacity with minimal friction. It provides you with complete control of your computing resources and lets you run on Amazon’s proven computing environment.
This allows you to build Infrastructure as a Service (IaaS) applications for instance-based virtual machines. You can provision virtual machines and manage them as you choose. This method of compute is a familiar concepts with IT professionals.
  * Containers
Amazon Web Services - has many different container services including Amazon Elastic Container Service, Amazon Elastic Kubernetes Service, AWS Fargate, and Amazon Elastic Container Registry. These services are instance-based and enable you to run multiple workloads on a single operating system (OS). Containers spin up more quickly than virtual machines, thus offering responsiveness. Container-based solutions continue to grow in popularity.
As a concept virtualization is not new to many IT professionals, however containers may be new. AWS Fargate can be used to help reduce administrative overhead and give you options for additional control.
  * Serverless
AWS Lambda - lets you run code without provisioning or managing servers. You pay only for the compute time you consume—there is no charge when your code is not running.
Serverless is a category of compute where you write and deploy code, but do not manage the underlying infrastructure.It is a function based environment that is low cost where deployed code can be triggered on a schedule or events. This is a newer concept for many IT professionals but is easy to learn and use.
  * Platform as a Service
Platform as a service - allows a company to focus on building code and applications rather than manage infrastructure. AWS Elastic Beanstalk provides a platform as a service (PaaS). It facilitates the quick deployment of applications that you create by providing all the application services that you need. AWS manages the OS, the application server, and the other infrastructure components so that you can focus on developing your application code.
For IT professionals, it is a fast and easy service to get started, however, you loose the ability to control the underlying infrastructure.
-------------------
Summary of AWS Compute Services
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

#### Choosing the Right Service

Selecting compute resources that meet your requirements, performance needs, and provide great efficiency of cost and effort will enable you to accomplish more with the same number of resources.

In AWS, compute is available in three forms: instances, containers, and functions:
  * Instances are virtualized servers, allowing you to change their capabilities with a button or an API call. Because resource decisions in the cloud aren’t ﬁxed, you can experiment with different server types. At AWS, these virtual server instances come in different families and sizes, and they offer a wide variety of capabilities, includ- ing solid-state drives (SSDs) and graphics processing units (GPUs).
  * Containers are a method of operating system virtualization that allow you to run an application and its dependencies in resource-isolated processes. AWS Fargate is serverless compute for containers or Amazon EC2 can be used if you need control over the installation, configuration, and management of your compute environment. You can also choose from multiple container orchestration platforms: Amazon Elastic Container Service (ECS) or Amazon Elastic Kubernetes Service (EKS).
  * Functions abstract the execution environment from the code you want to execute. For example, AWS Lambda allows you to execute code without running an instance.

Things that should be asked based on aspects of the project:
  * What is your application design?
  * What are your usage patterns? Consistent usage, infrequent usage?
  * Which configuration settings will you need to manage?

#### What are Virtual Machines?

A virtual machine (VM) - is a software-based computer that exists within another computer’s operating system, often used for the purposes of testing, backing up data, or running SaaS (Software as a Service) applications. 

Operating System - is what manages the computer’s hardware in ways that are useful to the user. For example, if the user wants to access the Internet, the OS directs the network interface card to make the connection. If the user wants to download a file, the OS will partition space on the hard drive for that file. The OS also runs and manages other pieces of software. For example, it can run a web browser and provide the browser with enough random access memory (RAM) to operate smoothly. Typically, operating systems exist within a physical computer at a one-to-one ratio; for each machine there is a single OS managing its physical resources.

Common examples of OSes are Mac OSX, Microsoft Windows, Linux, and Android.

Hypervisor - is a piece of software, firmware, or hardware that VMs run on top of. The hypervisors themselves run on physical computers, referred to as the “host machine”. The host machine provides the VMs with resources, including RAM and CPU. These resources are divided between VMs and can be distributed as you see fit. So if one VM is running a more resource heavy application, you might allocate more resources to that one than the other VMs running on the same host machine.

-------------------
What are virtual machines used for?

Some of the most popular reasons people run virtual machines include:
  * Testing - Oftentimes software developers want to be able to test their applications in different environments. They can use virtual machines to run their applications in various OSes on one computer. This is simpler and more cost-effective than having to test on several different physical machines.
  * Running software designed for other OSes - Although certain software applications are only available for a single platform, a VM can run software designed for a different OS. For example, a Mac user who wants to run software designed for Windows can run a Windows VM on their Mac host.
  * Running outdated software - Some pieces of older software can’t be run in modern OSes. Users who want to run these applications can run an old OS on a virtual machine
-------------------
How does cloud computing use virtual machines?

Several cloud providers offer virtual machines to their customers. These virtual machines typically live on powerful servers that can act as a host to multiple VMs and can be used for a variety of reasons that wouldn’t be practical with a locally-hosted VM. These include:
  * Running SaaS applications - Software-as-a-Service, is a cloud-based method of providing software to users. SaaS users subscribe to an application rather than purchasing it once and installing it. These applications are generally served to the user over the Internet. Often, it is virtual machines in the cloud that are doing the computation for SaaS applications as well as delivering them to users. If the cloud provider has a geographically distributed network edge, then the application will run closer to the user, resulting in faster performance.
  * Backing up data - Cloud-based VM services are very popular for backing up data, because the data can be accessed from anywhere. Plus, cloud VMs provide better redundancy, require less maintenance, and generally scale better than physical data centers. (For example, it’s generally fairly easy to buy an extra gigabyte of storage space from a cloud VM provider, but much more difficult to build a new local data server for that extra gigabyte of data.)
  * Hosting services like email and access management - Hosting these services on cloud VMs is generally faster and more cost-effective, and helps minimize maintenance and offload security concerns as well.

#### Introduction to EC2

Amazon Elastic Compute Cloud (Amazon EC2) provides virtual machines where you can host the same kinds of applications that you might run on a traditional on-premises server. It provides secure, resizable compute capacity in the cloud. EC2 instances can support a variety of workloads.

Common Server Uses:
  * Application servers
  * Catalog servers
  * Computing servers
  * File servers
  * Database servers
  * Game servers
  * Mail servers
  * Media servers
  * Proxy servers
  * Web servers
-------------------
Features & Terminology of Amazon EC2

Amazon EC2 provides the following features:
  * Virtual computing environments, known as instances 
  * Preconfigured templates for your instances, known as Amazon Machine Images (AMIs), that package the bits you need for your server (including the operating system and additional software)
  * Various configurations of CPU, memory, storage, and networking capacity for your instances, known as instance types
  * Secure login information for your instances using key pairs (AWS stores the public key, and you store the private key in a secure place)
  * Storage volumes for temporary data that's deleted when you stop or terminate your instance, known as instance store volumes 
  * Persistent storage volumes for your data using Amazon Elastic Block Store (Amazon EBS), known as Amazon EBS volumes
  * Multiple physical locations for your resources, such as instances and Amazon EBS volumes, known as Regions and Availability Zones 
  * A firewall that enables you to specify the protocols, ports, and source IP ranges that can reach your instances using security groups 
  * Static IPv4 addresses for dynamic cloud computing, known as Elastic IP addresses 
  * Metadata, known as tags, that you can create and assign to your Amazon EC2 resources
  * Virtual networks you can create that are logically isolated from the rest of the AWS cloud, and that you can optionally connect to your own network, known as virtual private clouds (VPCs)
-------------------
Key Benefits

Amazon documents the following key benefits which I hope you will see first-hand once we create and launch our instance by following the directions in this module.
Elastic Web-Scale Computing

Amazon EC2 enables you to increase or decrease capacity within minutes, not hours or days. You can commission one, hundreds, or even thousands of server instances simultaneously. You can also use Amazon EC2 Auto Scaling to maintain availability of your EC2 fleet and automatically scale your fleet up and down depending on its needs in order to maximize performance and minimize cost. To scale multiple services, you can use AWS Auto Scaling.

Completely Controlled

You have complete control of your instances including root access and the ability to interact with them as you would any machine. You can stop any instance while retaining the data on the boot partition, and then subsequently restart the same instance using web service APIs. Instances can be rebooted remotely using web service APIs, and you also have access to their console output.

Flexible Cloud Hosting Services

You have the choice of multiple instance types, operating systems, and software packages. Amazon EC2 allows you to select a configuration of memory, CPU, instance storage, and the boot partition size that is optimal for your choice of operating system and application. For example, choice of operating systems includes numerous Linux distributions and Microsoft Windows Server.

Integrated

Amazon EC2 is integrated with most AWS services such as Amazon Simple Storage Service (Amazon S3), Amazon Relational Database Service (Amazon RDS), and Amazon Virtual Private Cloud (Amazon VPC) to provide a complete, secure solution for computing, query processing, and cloud storage across a wide range of applications.

Reliable

Amazon EC2 offers a highly reliable environment where replacement instances can be rapidly and predictably commissioned. The service runs within Amazon’s proven network infrastructure and data centers. The Amazon EC2 Service Level Agreement commitment is 99.99% availability for each Amazon EC2 Region. 99.99% availability means Amazon is guaranteeing any downtime to be less than 4 minutes, 23 seconds in any month or approximately 52 minutes in a year.

Secure

Cloud security at AWS is the highest priority. As an AWS customer, you will benefit from a data center and network architecture built to meet the requirements of the most security-sensitive organizations. Amazon EC2 works in conjunction with Amazon VPC to provide security and robust networking functionality for your compute resources.

Inexpensive

Amazon EC2 passes on to you the financial benefits of Amazon’s scale. You pay a very low rate for the compute capacity you actually consume. See Amazon EC2 Instance Purchasing Options for more details.

Easy to Start

There are several ways to get started with Amazon EC2. You can use the AWS Management Console, the AWS Command Line Tools (CLI), or AWS SDKs.

#### EC2 Instance Types

Amazon EC2 provides a wide selection of instance types optimized to fit different use cases. Instance types comprise varying combinations of CPU, memory, storage, and networking capacity and give you the flexibility to choose the appropriate mix of resources for your applications. Each instance type includes one or more instance sizes, allowing you to scale your resources to the requirements of your target workload.

When launching an EC2 instance, one of the very first settings you need to select is to pick your instance type. Below is how you break down the names for the instance types, we will be using the t3.large instance type for this example:
  * The first letter T is the family name of the instance type, the famly name
  * The number after the letter is the generation number, so a T3 is the third generation in the T family
  * The last part after the period, is the size of the instance, which is a large 

General purpose instances - provides a broad balance of compute, memory and networking resources, and can be used for a variety of diverse workloads. These instances are ideal for applications that use these resources in equal proportions such as web servers and code repositories.

Compute Optimized instances - are ideal for compute bound applications that benefit from high performance processors. Instances belonging to this family are well suited for batch processing workloads, media transcoding, high performance web servers, high performance computing (HPC), scientific modeling, dedicated gaming servers and ad server engines, machine learning inference and other compute intensive applications.

Memory optimized instances - are designed to deliver fast performance for workloads that process large data sets in memory.

Accelerated computing instances - such as machine learning instances, use hardware accelerators, or co-processors, to perform functions, such as floating point number calculations, graphics processing, or data pattern matching, more efficiently than is possible in software running on CPUs.

Storage optimized instances - are designed for workloads that require high, sequential read and write access to very large data sets on local storage as part of a distributed file system. They are optimized to deliver tens of thousands of low-latency, random I/O operations per second (IOPS) to applications.

#### Amazon Machine Images (AMI)

Amazon Machine Images (AMI) - are pre-configured virtual machines with an ever-growing list of operating systems. These can help you get started faster and launch multiple instances from a single AMI.

An Amazon Machine Image (AMI) provides the information required to launch an instance. You must specify an AMI when you launch an instance. You can launch multiple instances from a single AMI when you need multiple instances with the same configuration. You can use different AMIs to launch instances when you need instances with different configurations.

An AMI includes the following:
  * One or more EBS snapshots, or, for instance-store-backed AMIs, a template for the root volume of the instance (for example, an operating system, an application server, and applications).
  * Launch permissions that control which AWS accounts can use the AMI to launch instances.
  * A block device mapping that specifies the volumes to attach to the instance when it's launched.

There are many different ways to use an AMI including:
1.	Quick Start AMI with Linux or Windows pre-built images provided by AWS
2.	My AMI that you created
3.	AWS Marketplace AMI  templates created by approved third parties and checked by AWS
4.	Community AMI created by individuals around the world. Use at your own risk as these have not been checked by AWS

#### Four Pillars of Cost Optimization

Regardless of your workload or architecture, there are four cost optimization pillars that apply across nearly all environments. The pillars of cost optimization are:

-------------------

Pillar 1. Right Size

Choose the right balance of instance types and ensure that what you provision matches what you need. Remember, you provision for CPU, memory, storage, and network throughput. It is important to notice when servers can be either sized down or turned off, and still meet your performance requirements.

For example, use Amazon CloudWatch metrics to deterine when compute resources are idle or can be downsized.

-------------------

Pillar 2. Increase elasticity

Traditional IT costs and hardware requirements are tailored for peak usage and are rarely turned off. In the cloud, you can optimize cost to meet dynamic needs and turn resources off when they are not needed. Automatic scaling can be utilized to match needs based on usage, automatically or based on a scheduled time.

For example, you can usually turn stop or hibernate non-production instances that are not actively in use.

-------------------

Pillar 3. Leverage the right pricing model

AWS provides a range of pricing models that can be combined to optimize pricing based on current or forecasted capacity needs. Choose the right pricing model to optimize costs based on the nature of your workload and usage patterns. For example, use on-demand or spot instances for variable workloads while using reserved instances for predictable workloads.

Customers are also encouraged to consider their application architecture. For example, does the functionality provided by your application need to run on an EC2 virtual machine? Perhaps by making use of the AWS Lambda service instead, you could significantly decrease your costs.

-------------------

Pillar 4. Optimize storage

AWS provides multiple storage tiers at prices designed to meet performance. Customers can also reduce storage costs through any combination of the following:
   * By identifying the most appropriate destination for specific types of data, you can reduce Amazon Elastic Block Store (Amazon EBS) and Amazon Simple Storage Service (Amazon S3) while maintaining the required performance and availability.
   * When you launch EC2 instances, different instance types offer different storage options. It is a best practice to try to reduce costs while also maintaining storage performance and availability. One way you can accomplish this is by resizing EBS volumes. For example, if you originally provisioned a 500-GB volume for an EC2 instance that will only need a maximum of 20 GB of storage space, you can reduce the size of the volume and save on costs.
   * There are also a variety of EBS volume types. Choose the least expensive type that still meets your performance requirements. For example, Amazon EBS Throughput Optimized HDD (st1) storage typically costs half as much as the default General Purpose SSD (gp2) storage option. If an st1 drive will meet the needs of your workload, take advantage of the cost savings.
   * Customers often use EBS snapshots to create data backups. However, some customers forget to delete snapshots that are no longer needed. Delete these unneeded snapshots to save on costs.

Finally, try to identify the most appropriate destination for specific types of data. Does your application need the data it uses to reside on Amazon EBS? Would the application run equally as well if it used Amazon S3 for storage instead? Configuring data lifecycle policies can also reduce costs. For example, you might automate the migration of older infrequently accessed data to cheaper storage locations, such as Amazon Simple Storage Service Glacier.

-------------------

Measure, monitor, and improve

To ensure that you extract the full economic potential of the AWS Cloud at any scale, you want to:
   * Define and enforce cost allocation tagging. Tagging helps provide information about what resources are being used by whom and for what purpose. You can activate cost allocation tags in the Billing and Cost Management console, and AWS can generate a cost allocation report with usage and costs grouped by your active tags. Apply tags that represent business categories (such as cost centers, application names, or owners) to organize your costs across multiple services.
   * Define metrics, set targets, and review at a reasonable cadence. Encourage teams to architect for cost. AWS Cost Explorer is a free tool that you can use to view graphs of your costs. You can use Cost Explorer to see patterns in how much you spend on AWS resources over time, identify areas that need further inquiry, and see trends that you can use to understand your costs.
   * Enable teams to architect for cost via training, visualization of progress goals, and a balance of incentives. Use AWS services such as AWS Trusted Advisor, which provides real-time guidance to help you provision resources that follow AWS best practices.
   * Assign optimization responsibility to an individual or to a team. Cost-optimization efforts are typically more successful when the responsibility for cost optimization is assigned to an individual or to a team.

-------------------

#### What are Containers?

A Container in cloud computing is an approach to operating system virtualization. By this, the user can work with a program and its dependencies using resource procedures that are isolated. The code of the application can be bundled with configurations and dependencies in a systematic manner.

Container in cloud computing is used to build blocks, which help in producing operational efficiency, version control, developer productivity and environmental consistency. Because of this, the user is assured of reliability, consistency, and quickness regardless of the distributed platform. The infrastructure is enhanced since it provides more control over the granular activities on resources. The container usage in online services benefits storage with cloud computing information security, availability and elasticity.

Benefits of Containerization

As a method of operating system virtualization, some of the benefits include:
   * Repeatable
   * Self-contained execution environment
   * Software runs the same in different environments (Development, Test, Production Servers)
   * Faster to launch and stop/ terminate environment than in virtual machines

Advantages of a Container in Cloud Computing

These are the following things that have to be provided by CASB solution (Links to an external site.):
   * The Consistency in Cloud Storage: The container enhances portability. It eliminates the organizational and technical frictions so that the program moves through the entire process cycle. It encapsulates the core files of an application and software server and dependencies like a building block. This can be distributed on any resource. The manual configuration of each server is thus completely avoided enabling the users to announce a new feature. 
   * Application Version Control: Through container in cloud computing, the users can look on the current version of the application code as well as their dependencies. A manifest file is managed by the Docker containers. The users can easily hold and track the editions of container, look for differences between the container editions and roll-back to earlier versions if needed. 
   * Efficiency in the Operational Activities: The users can achieve more resources through the container in cloud computing. By this, the users can also work at a time on several applications. The required memory, disk space and CPU consumed by the container have to be specified. Since each of the containers is a process of the operating system that works on an application and associated programs, the containers have a fast boot time. The users can quickly enter and exit the application and also measure it in up and down. The applications are separated from each other through the isolation procedure. This concept has no shared incompatibilities or dependencies. 
   * Productivity of the Developers: The containers deduct the dependencies and conflicts between the cross-service and thus the productivity increases. The component of the program is segregated into different entities that run a separate micro-service. There is no worry about the libraries and dependencies that are being synced for each service because the containers are isolated from each other. Each service can be upgraded independently as they are not in touch with each other.

#### What are Docker and Kubernetes?

Docker

A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. A Docker container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.

Container images become containers at runtime and in the case of Docker containers - images become containers when they run on Docker Engine. Available for both Linux and Windows-based applications, containerized software will always run the same, regardless of the infrastructure. Containers isolate software from its environment and ensure that it works uniformly despite differences for instance between development and staging.

Docker containers that run on Docker Engine:
   * Standard: Docker created the industry standard for containers, so they could be portable anywhere
   * Lightweight: Containers share the machine’s OS system kernel and therefore do not require an OS per application, driving higher server efficiencies and reducing server and licensing costs
   * Secure: Applications are safer in containers and Docker provides the strongest default isolation capabilities in the industry

-------------------
Kubernetes

Kubernetes is a portable, extensible, open-source platform for managing containerized workloads and services, that facilitates both declarative configuration and automation. It has a large, rapidly growing ecosystem. Kubernetes services, support, and tools are widely available.

Kubernetes enables you to deploy and manage containerized applications at scale. With Kubernetes, you can run any type of containerized application by using the same toolset in both on-premises data centers and the cloud. Kubernetes manages a cluster of compute instances (called nodes). It runs containers on the cluster, which are based on where compute resources are available and the resource requirements of each container. Containers are run in logical groupings called pods. You can run and scale one or many containers together as a pod. Each pod is given an IP address and a single Domain Name System (DNS) name, which Kubernetes uses to connect your services with each other and external traffic.

A key advantage of Kubernetes is that you can use it to run your containerized applications anywhere without needing to change your operational tooling. For example, applications can be moved from local on-premises development machines to production deployments in the cloud by using the same operational tooling.

-------------------
Docker vs Kubernetes

A fundamental difference between Kubernetes and Docker is that Kubernetes is meant to run across a cluster while Docker runs on a single node. Kubernetes is more extensive than Docker Swarm and is meant to coordinate clusters of nodes at scale in production in an efficient manner. Kubernetes pods—scheduling units that can contain one or more containers in the Kubernetes ecosystem—are distributed among nodes to provide high availability.

Here are the essential features of Docker:
  * Isolated environments for managing your applications
  * Easy Modeling
  * Version control
  * Placement/Affinity
  * Application Agility
  * Developer Productivity
  * Operational Efficiencies

Here are the essential features of Kubernetes:
  * Offers automated scheduling
  * Self-Healing capabilities
  * Automated rollouts & rollback
  * Horizontal Scaling & Load Balancing
  * Provides a higher density of resource utilization
  * Offers enterprise-ready features
  * Application-centric management
  * Auto-scalable infrastructure
  * You can create predictable infrastructure
  * Provides declarative configuration
  * Deploy and update software at scale
  * Offers environment consistency for development, testing, and production

#### What is Serverless Computing?

Serverless computing is a method of providing backend services on an as-used basis. Servers are still used, but a company that gets backend services from a serverless vendor is charged based on usage, not a fixed amount of bandwidth or number of servers.

A Serverless architecture allows users to write and deploy code without the hassle of worrying about the underlying infrastructure. A company that gets backend services from a serverless vendor is charged based on their computation and do not have to reserve and pay for a fixed amount of bandwidth or number of servers, as the service is auto-scaling. Note that although called serverless, physical servers are still used but developers do not need to be aware of them.
In the early days of the web, anyone who wanted to build a web application had to own the physical hardware required to run a server, which is a cumbersome and expensive undertaking.

Then came the cloud, where fixed numbers of servers or amounts of server space could be rented remotely. Developers and companies who rent these fixed units of server space generally over-purchase to ensure that a spike in traffic or activity wouldn’t exceed their monthly limits and break their applications. This meant that much of the server space that was paid for usually went to waste. Cloud vendors have introduced auto-scaling models to address the issue, but even with auto-scaling an unwanted spike in activity, such as a DDoS Attack, could end up being very expensive.

Cost Benefits of Serverless

Serverless computing allows developers to purchase backend services on a flexible ‘pay-as-you-go’ basis, meaning that developers only have to pay for the services they use. This is like switching from a cell phone data plan with a monthly fixed limit, to one that only charges for each byte of data that actually gets used.

The term ‘serverless’ is somewhat misleading, as there are still servers providing these backend services, but all of the server space and infrastructure concerns are handled by the vendor. Serverless means that the developers can do their work without having to worry about servers at all.

What are backend services? What’s the difference between frontend and backend?

Application development is generally split into two realms: the frontend and the backend. The frontend is the part of the application that users see and interact with, such as the visual layout. The backend is the part that the user doesn’t see; this includes the server where the application's files live and the database where user data and business logic is persisted.

1.	Front End: Requests Website Data
2.	Back End: Responds with Website Data
3.	Front End: Displays website, forwards reqeusts for concert dates
4.	Back End: Checks database, delivers list of available dates and tickets
5.	Front End: Requests website data
6.	Back End: Updates database of tickets, processes payment, sends confirmation info

What kind of backend services can serverless computing provide?

Most serverless providers offer database and storage services to their customers, and many also have Function-as-a-Service (FaaS) platforms, like Cloudflare Workers. These platforms can execute pieces of code on the edge without storing any data.

What are the advantages of serverless computing?

  * Lower costs - Serverless computing is generally very cost-effective, as traditional cloud providers of backend services (server allocation) often result in the user paying for unused space or idle CPU time.
  * Simplified scalability - Developers using serverless architecture don’t have to worry about policies to scale up their code. The serverless vendor handles all of the scaling on demand.
  * Simplified backend code - With FaaS, developers can create simple functions that independently perform a single purpose, like making an API call.
  * Quicker turnaround - Serverless architecture can significantly cut time to market. Instead of needing a complicated deploy process to roll out bug fixes and new features, developers can add and modify code on a piecemeal basis.






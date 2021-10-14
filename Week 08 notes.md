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





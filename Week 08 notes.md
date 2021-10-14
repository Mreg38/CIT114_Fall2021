# CIT 114 Week 8
## Here are some important thinkgs I learned in Week 8
### Notes 06: Compute

#### What is an Operating System

An operating system is the most important software that runs on a computer. It manages the computer's memory and processes, as well as all of its software and hardware. It also allows you to communicate with the computer without knowing how to speak the computer's language. Without an operating system, a computer is useless.

Operating system (OS) manages all of the software and hardware on the computer. Most of the time, there are several different computer programs running at the same time, and they all need to access your computer's central processing unit (CPU), memory, and storage. The operating system coordinates all of this to make sure each program gets what it needs.

Operating systems usually come pre-loaded on any computer you buy. Most people use the operating system that comes with their computer, but it's possible to upgrade or even change operating systems. The three most common operating systems for personal computers are Microsoft Windows, macOS, and Linux.

Modern operating systems use a graphical user interface, or GUI (pronounced gooey). A GUI lets you use your mouse to click icons, buttons, and menus, and everything is clearly displayed on the screen using a combination of graphics and text.

Microsoft created the Windows operating system in the mid-1980s. There have been many different versions of Windows, but the most recent ones are Windows 10 (released in 2015), Windows 8 (2012), Windows 7 (2009), and Windows Vista (2007). Windows comes pre-loaded on most new PCs, which helps to make it the most popular operating system in the world.

Linux (pronounced LINN-ux) is a family of open-source operating systems, which means they can be modified and distributed by anyone around the world. This is different from proprietary software like Windows, which can only be modified by the company that owns it. The advantages of Linux are that it is free, and there are many different distributions—or versions—you can choose from.

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











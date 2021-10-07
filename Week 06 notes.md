# CIT 114 Week 6 (Notes 04: Cloud Security)
## Here are some important thinkgs I learned in Week 6
### Cloud Security

#### What is Cyber Security?

Cybersecurity is the art of protecting networks, devices, and data from unauthorized access or criminal use and the practice of ensuring confidentiality, integrity, 
and availability of information. It seems that everything relies on computers and the internet now—communication (e.g., email, smartphones, tablets), entertainment 
(e.g., interactive video games, social media, apps ), transportation (e.g., navigation systems), shopping (e.g., online shopping, credit cards), medicine 
(e.g., medical equipment, medical records), and the list goes on.

What are the risks to having poor cybersecurity?

Dangers are malware erasing your entire system, an attacker breaking into your system and altering files, an attacker using your computer to attack others, or an 
attacker stealing your credit card information and making unauthorized purchases. There is no guarantee that even with the best precautions some of these things won't 
happen to you, but there are steps you can take to minimize the chances.

Terms to better understand the risks:
  * Hacker, attacker, or intruder – These terms are applied to the people who seek to exploit weaknesses in software and computer systems for their own gain. Although 
their intentions are sometimes benign and motivated by curiosity, their actions are typically in violation of the intended use of the systems they are exploiting
  * Malicious code – Malicious code (also called malware) is unwanted files or programs that can cause harm to a computer or compromise data stored on a 
computer. Various classifications of malicious code include viruses, worms, and Trojan horses
      
      Malicious code may have the following characteristics:
      * It might require you to actually do something before it infects your computer. This action could be opening an email attachment or going to a particular webpage.
      * Some forms of malware propagate without user intervention and typically start by exploiting a software vulnerability. Once the victim computer has been infected, 
      the malware will attempt to find and infect other computers. This malware can also propagate via email, websites, or network-based software.
      * Some malware claims to be one thing, while in fact doing something different behind the scenes. For example, a program that claims it will speed up your computer 
      may actually be sending confidential information to a remote intruder.

  * Vulnerabilities – Vulnerabilities are flaws in software, firmware, or hardware that can be exploited by an attacker to perform unauthorized actions in a system. They can be caused by software programming errors

To minimize the risks of cyberattacks, follow basic cybersecurity best practices:
  * Keep software up to date
  * Run up-to-date antivirus software
  * Use strong passwords
  * Change default usernames and passwords
  * Implement multi-factor authentication (MFA)
  * Install a firewall
  * Be suspicious of unexpected emails

#### AWS responsibility “Security of the Cloud”

AWS is responsible for protecting the infrastructure that runs all of the services offered in the AWS Cloud. This infrastructure is composed of the hardware, software, networking, and facilities that run AWS Cloud services. This includes:

  * Physical security of data centers with controlled, need-based access; located in nondescript facilities, with 24/7 security guards; two-factor authentication; access logging and review; video surveillance; and disk degaussing and destruction.
  * Hardware infrastructure, such as servers, storage devices, and other appliances that AWS relies on.
  * Software infrastructure, which hosts operating systems, service applications, and virtualization software.
  * Network infrastructure, such as routers, switches, load balancers, firewalls, and cabling. AWS also continuously monitors the network at external boundaries, secures access points, and provides redundant infrastructure with intrusion detection.

#### Customer responsibility “Security in the Cloud”

Inherited Controls – Controls which a customer fully inherits from AWS.
  * Physical and Environmental controls

Shared Controls – Controls which apply to both the infrastructure layer and customer layers, but in completely separate contexts or perspectives. In a shared control, AWS provides the requirements for the infrastructure and the customer must provide their own control implementation within their use of AWS services. Examples include:
  * Patch Management – AWS is responsible for patching and fixing flaws within the infrastructure, but customers are responsible for patching their guest OS and applications.
  * Configuration Management – AWS maintains the configuration of its infrastructure devices, but a customer is responsible for configuring their own guest operating systems, databases, and applications.
  * Awareness & Training - AWS trains AWS employees, but a customer must train their own employees.

Customer Specific – Controls which are solely the responsibility of the customer based on the application they are deploying within AWS services. Examples include:
  * Service and Communications Protection or Zone Security which may require a customer to route or zone data within specific security environments.
  * What content they choose to store on AWS
  * Which AWS services are used with the content
  * In what country that content is stored
  * The format and structure of that content and whether it is masked, anonymized, or encrypted
  * Who has access to that content and how those access rights are granted, managed, and revoke

AWS Identity and Access Management (IAM) is a web service that helps you securely control access to AWS resources for your users. You use IAM to control who can use your AWS resources (authentication) and what resources they can use and in what ways (authorization).

Authorization in IAM

Authorization is the process of determining what permissions a user, service or application should be granted. After a user has been authenticated, they must be authorized to access AWS services.

The principle of least privilege is an important concept in computer security. It promotes that you grant only the minimal user privileges needed to the user, based on the needs of your users. When you create IAM policies, it is a best practice to follow this security advice of granting least privilege.

How IAM Determines Permissions

1.	A request is made to IAM to access a service.
2.	IAM checks if permission to the service is explicitly denied. 
   *	If yes, the request is denied and process ends
   *	If no, the request moves to the next check
3.	IAM then checks if permission is explicitly allowed. 
   *	If yes, the request is allowed and the request continues to the service
   *	If no, the request receives an implicit deny and the process ends

Features of IAM:
  * Shared access to your AWS account - You can grant other people permission to administer and use resources in your AWS account without having to share your password or access key
  * Granular permissions - You can grant different permissions to different people for different resources
  * Secure access to AWS resources for applications that run on Amazon EC2 - You can use IAM features to securely provide credentials for applications that run on EC2 instances. These credentials provide permissions for your application to access other AWS resources
  *	Multi-factor authentication (MFA) - You can add two-factor authentication to your account and to individual users for extra security
  *	Identity federation - You can allow users who already have passwords elsewhere—for example, in your corporate network or with an internet identity provider—to get temporary access to your AWS account
  *	Identity information for assurance - If you use AWS CloudTrail  (Links to an external site.), you receive log records that include information about those who made requests for resources in your account
  *	PCI DSS Compliance - IAM supports the processing, storage, and transmission of credit card data by a merchant or service provider, and has been validated as being compliant with Payment Card Industry (PCI) Data Security Standard (DSS)
  *	Integrated with many AWS services
  *	Eventually Consistent - IAM, like many other AWS services, is eventually consistent  (Links to an external site.). IAM achieves high availability by replicating data across multiple servers within Amazon's data centers around the world. If a request to change some data is successful, the change is committed and safely stored
  *	Free to use - AWS Identity and Access Management (IAM) and AWS Security Token Service (AWS STS) are features of your AWS account offered at no additional charge. You are charged only when you access other AWS services using your IAM users or AWS STS temporary security credentials

#### Essential Elements of IAM

IAM User

An IAM user can be assigned either:
  * Programmatic access via the AWS Command Line Interface (CLI) or AWS Software Development Kit (SDK) 
  * AWS Management Console access via IAM were a 12 digit Account ID, IAM Username, and IAM Password are assigned with optional multi-factor authentication (MFA).

IAM Group

Some important characteristics of IAM groups include:
  * A group can contain many users, and a user can belong to multiple groups.
  * Groups cannot be nested. A group can contain only users, and a group cannot contain other groups.
  * There is no default group that automatically includes all users in the AWS account. If you want to have a group with all account users in it, you need to create the group and add each new user to it.

IAM Policy - a document that defines permissions to determine what users can do in the AWS account. A policy typically grants access to specific resources and specifies what the user can do with those resources. Policies can also explicitly deny access

IAM Role - a tool for granting temporary access to specific AWS resources in an AWS account. An IAM role is similar to an IAM user because it is also an AWS identity that you can attach permissions policies to, and those permissions determine what the identity can and cannot do in AWS

#### Four Ways to use IAM

You can work with AWS Identity and Access Management in any of the following ways

AWS Management Console:

The console is a browser-based interface to manage IAM and AWS resources. For more information about accessing IAM through the console

AWS Command Line Tools:

You can use the AWS command line tools to issue commands at your system's command line to perform IAM and AWS tasks. Using the command line can be faster and more convenient than the console. The command line tools are also useful if you want to build scripts that perform AWS tasks. AWS provides two sets of command line tools: the AWS Command Line Interface (AWS CLI) and the AWS Tools for Windows PowerShell

AWS SDKs:

AWS provides SDKs (software development kits) that consist of libraries and sample code for various programming languages and platforms (Java, Python, Ruby, .NET, iOS, Android, etc.). The SDKs provide a convenient way to create programmatic access to IAM and AWS

IAM HTTPS API:

You can access IAM and AWS programmatically by using the IAM HTTPS API, which lets you issue HTTPS requests directly to the service. When you use the HTTPS API, you must include code to digitally sign requests using your credentials

#### Security Services

  * AWS Service Catalog - allows organizations to create and manage catalogs of IT services that are approved for use on AWS. These IT services can include everything from virtual machine images, servers, software, and databases to complete multi-tier application architectures.
  * AWS Web Application Firewall (WAF) - helps protect your web applications or APIs against common web exploits that may affect availability, compromise security, or consume excessive resources. This differs from AWS Shield in that it operates on application layer (Layer 7) of the OSI model and protects against attacks such as SQL injection or cross-site scripting.
  * Amazon Macie - is a fully managed data security and data privacy service that uses machine learning and pattern matching to discover and protect your sensitive data in AWS. It can help you proactively identify and protect personally identifiable information (PII) and know when it moves.
  * Amazon Inspector - is an automated security assessment service that helps improve the security and compliance of applications deployed on AWS. Amazon Inspector automatically assesses applications for exposure, vulnerabilities, and deviations from best practices. It can help you validate you are adhering to standards.
  * Amazon GuardDuty - is an intelligent threat detection service that continuously monitors for malicious activity and unauthorized behavior to protect your AWS accounts and workloads.


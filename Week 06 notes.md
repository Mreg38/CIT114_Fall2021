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
   1.	If yes, the request is denied and process ends
   2.	If no, the request moves to the next check
3.	IAM then checks if permission is explicitly allowed. 
   1.	If yes, the request is allowed and the request continues to the service
   2.	If no, the request receives an implicit deny and the process ends




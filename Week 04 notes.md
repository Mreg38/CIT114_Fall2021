# CIT 114 Week 4
## Here are some important things I learned in Week 4
### Cloud Economics, Billing & Support

#### Amazon Web Services (AWS)
- Ability to let one optimize costs to match needs, even as needs change
- Pay-as-you-go (on demand), reservation-based and bulk-use (pay less when you use more) payment models

#### Key Principles of Pricing
3 Fundamental drivers of cost with AWS:
1. Compute
2. Storage
3. Outbound data transfer

How to deal with those cost drivers:
- Start early with cost optimization
- Maximize the power of flexiblity
- Use the right pricing model for the job

#### The right pricing model for the job
- On Demand: pay for tcompute or database capacity with no long-term commitments or upfront payments
- Dedicated Instances (available with Amazon [Elastic Compute Cloud](https://aws.amazon.com/ec2/?ec2-whats-new.sort-by=item.additionalFields.postDateTime&ec2-whats-new.sort-order=desc)) (Amazon EC2): run in a virtual private cloud (VPC) on hardware that's dedicated to a single customer.
- Spot Instances: an Amazon EC2 pricing mechanism that lets you purchase spare computing capacity with no upfront commitment at discounted hourly rates
- Reservations: provide you with the ablity to receiver a greater discount by paying for capacity ahead of time.

#### Free Tier of Service
|Resource|Description|
|:---|:---|
|AWS Credits|$25 in credits for your normal AWS account, if requested|
|AWS Educate|$100 in credits for a starter account and access to classrooms with additional credits|
|AWS Training|Access to AWS Technical Essentials Training Course and free access to labs|
|Content|Ability to select personalized learning pathway with 30+ hours of content per path. Earn digital badges that showcase cloud skills. Free access to AWS content for homework, labs or self-study|
|Collaboration|Student Portal access. Student Portfolio to store developed projects in one place. Access to the AWS Job Board and job postings|

#### AWS Services with no charge
- Amazon Virtual Private Cloud (Amazon VPC) AWS Identify and Access Management (IAM)
- Consolidated Billing
- AWA Elastic Beanstalk
- AWS CloudFormation
- Automatic Scalling 
- AWS OpsWorks

#### IT Infrastructure
- Components of IT infrastructure
  - Hardware
  - Software
  - Networking
- Types of IT Infrastructure
  - Traditional
  - Cloud

#### Total Cost of Ownership (TCO)
A formula that assess direct and indirect costs and benefits related to the purchase of any IT component.
- Models for different cloud providers
  - TCO is domain- or enterprise-dependent
  - Real benefit is ability to react to changing business needs
  - We have to consider our existing investments!
- Defining our own TCO model
  - Existing infrastructure
  - Existiing skills and humans
  - Difference in costs, pre-cloud to post-cloud
  - Cost of cloud services whein in operations
  - Value of agility (including time-to-market)
  - Value of avoiding future capital expenditures
  - Cost of risk around compliance issues
- Components of Total Cost for Technology
  - Hardware acquisition
  - Software acquisition
  - Infrastructure
  - Downtime
  - Installation
  - Maintenance
  - Training
  - Support
  - Space
  - Electricity

#### AWS Organizations: Terminology
- Organization: Entity created to consolidate AWS accounts.
- Root: Parent container for all the accounts for your organization.
- Organization unit (OU): A container for accounts within a root. Can containother OUs, enabing you to create a hierarchy that looks like an upside-down tree.
- Accounts: A standard AWS account that contains your AWS resources. You can attach a policy to an account to apply control  ton only that one account.
  - Master account: Account that creates the organization.
  - Member account: The rest of the accounts that belong to an organization. Can only be a member of one organization at a time.
- Invitation: Process of asking another account to join your organization. Can only be issued by the organization's master account.
- Handshake: Multi-step process of exchanging information between two parties.

#### Steps to Create an Organization
1. Create organization
2. Create organizational units
3. Create service control policies
4. Test restrictions

#### Support Plan Features & Prices
4 levels of support plans
1. Basic Support Plan
The Basic plan costs nothing and provides limited support.
- 24/7 access to customer service, documentation, white papers and white papers and support forums.
- Access to six core Trusted Advisor checks.
- Access to the Personal Health Dashboard.
2. Developer Support Plan
Offers resources for customers testing or doing early development on AWS, as well as any customers who:
- Want access to guidance and technical support.
- Are exploring how to quickly put AWS to work.
- Who use AWS for non-production workloads or applications.
3. Business Support Plan
Offers resources for customers running production workloads on AWS as well as any customers who:
- Run one or more applications in production environments.
- Have multiple services activated, or use key services extensively.
- Depend on their business solutions to be available, scalable and secure.
4. Enterprise Support Plan
Offers resources for customers running business and mission-critical workloads on AWS, as well as customers who want to:
- Focus on proactive management to increase efficiency and availability.
- Build and operate workloads following AWS best practices.
- Leverage AWS expertise to support launches and migrations.
- Use a Technical Account Manager to provide technical expertise for the full range of AWS services and obtain a detailed understanding of your use case and technology architecture. The Technical Account Manager is the primary point of contact for ongoing needs.


# CIT 114 Week 12

## Here are some important thinkgs I learned in Week 12
### Notes 10: Automatic Scaling & Monitoring

#### CloudWatch Terminology

   * Namespace - Each AWS service stores its CloudWatch metrics and associated data in its own container. At this writing, there are more than 74 AWS services that use CloudWatch metrics.
   * Metrics - Each metric is a variable within an AWS. Each monitored variable produces a data set that is collected over a time period resulting in a graph defined by data points. The data points represent the metric data received from the variable being monitored at an exact point in time based on the range of times selected. For example, with EC2 instances, you can monitor the metric CPU usage. Over the last hour, which is shown on the x-axis, the data points represent the data collected over the last hour in 5-minute increments, defined as the period of time. The y-axis shows the percentage of CPU utilization.
   * Statistics - Each metric that you select for analysis collects data based on a defined time period.
   Graphed data will be categorized statistically using some of the following terms:
      - Minimum - The lowest value seen during the specified time period.
      - Maximum - The highest value seen during the specified time period.
      - Sum - All values are added together based on a specific time period.
      - SampleCount - The number of data points over a time period.
      - Average - Calculated from Sum divided by SampleCount based on the time period.
   * Dimensions - A dimension describes the metric and what data it stores. Multiple dimensions can be multiple instances assigned to the metric CPU utilization.
   * Units of measurement - Statistics are defined by bytes, seconds, count, or percentage.
   * Timestamp - Each metric is stamped with a timestamp that references the exact time when data was received. Each timestamp includes the date, hours, minutes, and seconds based on the current time in UTC format.
   * Time Range (Period) - The length of time data is collected based on a metric calculated on the defined statistical value. Periods of time can be set from 1 minute up to 15 months. The number of periods define the number of data points that are presented on the graph.
   * Alarms - An alarm starts an action based on the state of the metric’s data over the defined time. Alarms can be notifications using SNS topics, an EC2 action, or an auto scaling action. Each of the CloudWatch metric’s data output can also be analyzed against a custom baseline of defined measurement; if the data is below a defined threshold, all is well. However, once the metric’s results exceed the baseline or exceed the baseline for a defined time period, CloudWatch alarms can fire, notifying you that there’s potentially an issue. Even better, CloudWatch can alert another AWS service that there’s a problem, and the problem can be fixed—automatically in some cases. Once enabled, every CloudWatch alarm has three possible states:
      - OK - This means that the associated metric is still okay; the data that has been collected and evaluated by CloudWatch still fits within the defined alarm threshold. For example, you may have defined the CPU utilization at 60%. CloudWatch’s analysis of the metric’s data points over a defined evaluation period indicates that CPU utilization is currently at 52%; therefore, everything’s still okay.
      - ALARM - Everything’s not okay; the metric’s data indicates that the established baseline of acceptable CPU utilization has been breached.
      - INSUFFICIENT DATA - Everything might still be okay; there’s just not enough data yet to make a definitive analysis.
   * Events - CloudWatch provides near real-time stream of system events for most AWS services based on a defined pattern, such as API calls indicating Root account usage within the AWS account or any IAM API calls. The stream can be stored in a CloudTrail log group and tracked by a metric filter. The target that is notified when the event rule fires can be several AWS services, including an SNS topic, a Lambda function, or an SQS queue. Terra Firma can use events to track any issues with user authentication to AWS.

------

Elastic Load Balancing

   * Load Balancing --> Spreads out network traffic among multiple servers
   * Also provides redundancy --> One server goes down, not breaks in servives
   * Most AWS Services are offered with a "built-in" redundancy... EXCEPT for EC2!!

Options:
   * cation Load Balancer (ALB)
   * Network Load Balancer (NLB)
   * ELB is Redundant
   * EC2 Health Checks
   * Other features:
      -	SSL/TLS Traffic Decryption
      -	IPv4 or v6 support
      -	Dynamic port mapping
      -	Connection draining
      -	Cross-AZ support
      -	User authentication

------

Application + Network Load Balancing

  *	Distributes incoming traffic across multiple EC2 instances
  *	Listener --> Checks for connection requests from clients, and forwards requests to a target group
  *	Target Group --> Where the requests go
  *	DIFFERENCE between ALB/NLB:
    -	NLB --> Distributes traffic based on network variables, ie. IP addresses and destination ports.
    -	ALB --> Distributes requests based on multiple variables, INCLUDING network variables; ex. behavior of the application.

Auto Scaling
  *	EC2 auto scaling --> Allows us to launch or terminate instances controlled by CloudWatch alarms. Metrics include auto-scale group metrics such as the minimum and maximum group size and the in-service, pending, standby, and total instances.
  *	AWS auto scaling --> Supports services outside of EC2, including database services.

------

Useful features of CloudWatch to consider implementing:

  *	Auto scaling with CloudWatch alarms—Automatically adjust your applications based on need with EC2 auto scaling, ELB, and CloudWatch alarms.
  *	Filter logs with metric filters and alerts—Be notified when specific data patterns occur in your logs, and act accordingly using CloudWatch alerts, metric filters, and simple notification service (SNS) notifications calling Lambda to run custom functions for custom tasks.
  *	Billing alarms enabling you to monitor costs—Control costs by matching billing alerts to actual budget targets using billing alerts and SNS notifications.
  *	Logging CloudTrail IAM API calls to CloudWatch logs—This involves creating CloudTrail trails, storing the trails in CloudWatch, and using metric filters on root account activity.

------

What Is CloudWatch?

CloudWatch is a monitoring service embedded in the AWS cloud operating system. Many AWS services use CloudWatch to collect metrics that you can use to analyze how your service is currently operating. After ordering specific AWS services, metrics are enabled and available for evaluating the performance and operation of most AWS services, including EC2 instances, EBS volumes, Elastic Load Balancers (ELBs), Auto Scaling groups (ASGs), relational database service (RDS) DB instances, DynamoDB tables, Route 53 health checks, SNS topics and Simple Queue Service (SQS) queues, Storage Gateways, and S3 buckets. Only once an AWS service has been ordered and begins operation is there any data flow, and subsequently, CloudWatch metric data records published to the service’s CloudWatch dashboard.

Monitoring

Basic monitoring provided by CloudWatch is free of charge and, depending on the AWS service, a select number of metrics are enabled. Metrics report to CloudWatch on a variety of intervals. There is no default among all the services that are supported. For example, for EC2 instances and containers (elastic container service [ECS]), metric data is sent to CloudWatch every 5 minutes. For RDS databases and ELB, a selection of metric data is sent to CloudWatch every 60 seconds. EC2 instances also can enable detailed monitoring, which increases the reporting period to every 60 seconds; however, detailed monitoring is not free.

There’s no exact rhyme or reason as to why there are initial differences between the exact number of metrics that are bundled with each AWS service for basic monitoring. Make sure to check what basic monitoring options are available for each service in the AWS documentation; new metrics are being added to CloudWatch all the time, further enhancing its monitoring ability. With every AWS service, there are additional metrics you can choose to also use in monitoring.

Logging

CloudWatch also has a logging service that allows you to send your log data from your Linux and Windows instances to CloudWatch log groups. This enables you to further analyze and search your log data for any specific patterns, such as errors or system issues, that you want to analyze further

The CloudTrail managed service tracks all API calls made to an AWS account for 90 days. The creation of “trails” allows you to send all CloudTrail event information to a CloudWatch log group. CloudWatch log data can also be monitored by creating a metric filter that looks for a specific data pattern or patterns. Once a matching data pattern is found, a CloudWatch alarm can fire off an SNS notification about the issues that have been found (for example, 404 status codes in an Apache access log).

Another example of CloudWatch log groups is a virtual private cloud (VPC) network feature called VPC flow logs. Once those logs are enabled, network traffic can be captured from a single network adapter, a single subnet, or all network traffic within a VPC to a CloudWatch log group, providing the ability to analyze your network traffic.
Collected data stored in a CloudWatch log can be analyzed further by selecting one of the following options:

   * Export log data to Amazon S3—Log information on a defined date range can be exported to a Simple Storage Service (S3) bucket for analysis by any third-party monitoring application.
   * Stream log data to AWS Lambda—When a log event matches a specific filter, Lambda can swing into action and carry out its defined task. Amazon warns you that streaming log data might cost you; it recommends creating a budget that alerts you when you are close to exceeding your defined budget.
   * Stream to an Amazon ElastiSearch Cluster—Do this and visualize your data using the open source data virtualization tool Kibana.

------

Planning for Monitoring

When deciding what to monitor, the best suggestion is to keep it simple when first starting. If you make it too complicated in the beginning, you’ll probably give up. We are monitoring because we want to know when our AWS services are not operating as we expect. Perhaps the service seems slow and we want to understand why. We are ultimately monitoring to be kept abreast of potential problems before they occur and when problems occur. Monitoring allows us to become proactive in solving problems. Monitoring also allows us to proactively react to problems through automation.
Also, it won’t be obvious at first, but after you start monitoring and evaluating the results, the light will turn on; your data will indicate what trends are happening, and you will begin to discover why monitoring your applications is essential.

The types of things you can monitor include the following:
   * Performance-based monitoring—Monitoring your application’s compute speed (database, application, or Web server) over time allows you to develop your own initial baseline of operation and what you deem to be an acceptable level of performance. For example, monitoring an application server over a longer time period—for multiple weeks or months—provides valuable data insights as to when the application server gets busy, when there are quiet times, and whether it is busier at the end of the month or at certain times of day. The same criteria can apply to a Web server or a database server. EC2 instances, ECS containers, and RDS instances have CloudWatch metrics; in fact, all AWS services have some integration with CloudWatch.
   * Resources to Monitor—The initial components to monitor with regard to compute performance are the same ones we have always monitored: CPU, memory, storage, and networking.
   * CPU and RAM utilization—EC2 instances have the CloudWatch agent installed, which collects many system metrics from EC2 instances. On EC2 instances running Windows Server, all counters in Performance Monitor can be collected by the CloudWatch agent. Linux instances collect system information using metrics for CPU, disk, memory, and networking.
   * Available disk space—Hard disks with more than 70% disk space used are typically on the edge of causing problems due to lack of available free space. EBS volumes have disk performance and disk read and write operation metrics, and the CloudWatch agent can report on total disk space, used space, percentage of total disk space, and many other metrics. We can also quickly scale our EBS drives at AWS.
   * IOPS—CloudWatch has metrics for EBS volumes. In addition, the overall read and write performance of EBS volumes can be monitored and increased if necessary by raising input/output per second (IOPS) performance to 64,000 IOPS.
   * Network traffic—Traffic includes subnet traffic but can also include load-balancing and connections to the cloud, including VPN connections and Direct Connect connections. CloudWatch metrics are available for the ELB service, network address translation (NAT) gateway, transit gateway, and VPN connections. VPC flow logs also capture pertinent network information that is stored at CloudWatch. Additional metrics are available for EC2 instance networking.

------

CloudWatch Integration

The following list details some of the AWS services that are embedded with CloudWatch:

   * SNS—It is used for communication to humans or to other AWS services for sending automated alerts when CloudWatch alarms or events fire.
   * ELB—Load balancer metrics include active connection count, request count, healthy host count, transport layer security (TLS) connection errors, HTTP responses, and errors.
   * S3 buckets—Storage metrics detail the number of objects and bucket size; request metrics include all requests, get requests, bytes uploaded and downloaded, 4xx errors, and 5xx errors.
   * EC2 instances—Once an instance has been launched from the Monitoring tab, 14 metrics are displayed. These include options for CPU utilization and credits, disk read and write operations, network traffic and packet flow, and status checks.
   * EC2 auto scaling—This allows you to launch or terminate instances controlled by CloudWatch alarms. Metrics include auto-scale group metrics such as the minimum and maximum group size and the in-service, pending, standby, and total instances.
   * CloudTrail—After a trail has been created, CloudWatch writes the API calls fired in your AWS account to a CloudWatch log file stored in an S3 bucket.
   * AWS Config—All evaluated rules that fall out of compliance can invoke CloudWatch alarms, which in turn call Lambda.
   * RDS—Metrics include database connections, disk queue length, free storage space, read and write throughput, solid-state drive (SSD) burst balance, and CPU credit usage.
   * IAM—All authentication attempts, both successful and unsuccessful, can be monitored by a CloudWatch alarm. When the alarm is fired, SNS notifications can notify humans and automated responses.
   * Trusted Advisor—metrics include color-codes: green (good), red (there’s issues to check), and yellow (there’s warnings to consider).
   * VPC—Metrics include NAT and transit gateways.


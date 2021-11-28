# CIT 114 Week 12

## Here are some important thinkgs I learned in Week 12
### Notes 10: Automatic Scaling & Monitoring

#### CloudWatch Terminology

   * Namespace
   * Metrics
   * Statistics
      - Minimum
      - Maximum
      - Sum
      - SampleCount
      - Average
   * Dimensions
   * Units of measurement
   * Timestamp
   * Time Range (Period)
   * Alarms
      - OK
      - ALARM
      - INSUFFICIENT DATA
   * Events

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

Vice President, Amazon Elastic Compute Cloud (Amazon EC2)

David Brown joined AWS in 2007 as a software developer based in Cape Town, South Africa, working on the early development of Amazon EC2—a web service that provides secure, resizable compute and networking capacity in the cloud. Over the last 15 years, he’s held several roles within the Amazon EC2 organization, shaping the service into what it is today. Prior to joining AWS, David worked as a software developer within a financial industry startup.
### The power of cloud network innovation

From the very beginning, the AWS network has been the foundation for how AWS delivers on the promise of cloud computing. In this talk, join Dave Brown, VP of Amazon EC2 Networking and Compute Services, as he looks at the history of AWS networking and how its growth and innovation continues to this day—helping unleash your creativity and make leaps forward in what’s possible. With a combination of real-world examples and looks behind the scenes, Dave dives into the latest innovations in AWS core networking infrastructure, VPC networking, data center networking for AI/ML, security, and global connectivity.

### Networking Matters
1440 Germany Gutenberg printing press

Ada Palmer "You printed 200 copies of the Bible, there are three people in town who can read."

Venice was a better market, shipping and distribution network carried the books around the world.

Without connectivity it's hard to succeed.

Connectivity drives collaboration, and collaboration drives innovation.

AWS Backbone, 5,000,000km of fiberoptic backbone

74 Zettabytes per year

![[Pasted image 20231127160503.png]]

![[Pasted image 20231127160527.png]]

Region expansion benefits

![[Pasted image 20231127160605.png]]

How AWS regions are different


![[Pasted image 20231127160707.png]]

Local Zones
![[Pasted image 20231127160752.png]]

They make "movie shows" - using Local Zone GPUs on AWS

LA Local Zone 1-2ms latency

Direct Connect colocation sites now over 130, globally.
(100Gbps)

Cloudfront is 15 years old
- 600 points of presence
- 3 trillion requests per day

120Tbps peak during the NotFL SuperbOwl

Telegraph was the first computer network

AWS Nitro architecture behind EC2

![[Pasted image 20231127161425.png]]

Uses no part of central machine resources for their internal workloads. 

This is hardware-based hypervisor virtualization.

400Gbps 2020 with C7GN instances.

All enabled by Nitro

AI/ML workloads P4d, A100 GPU 400Gbps

Now line go up....

![[Pasted image 20231127161652.png]]

AMD H100GPU 32000Gbps on a single EC2 instance

![[Pasted image 20231127161734.png]]

It's a lot

![[Pasted image 20231127161807.png]]

Up to 50 Petabits per second?
![[Pasted image 20231127161852.png]]

AI/ML scale is pushing network topology design

![[Pasted image 20231127161928.png]]

![[Pasted image 20231127161954.png]]

![[Pasted image 20231127162024.png]]

64,000 GPUs per cluster? what? eeeeeeee!

![[Pasted image 20231127162109.png]]

Very important to count hops for latency prediction

![[Pasted image 20231127162144.png]]

Topology API gives information on relative network fabric topology

Trad TCP routing

![[Pasted image 20231127162228.png]]

New AWS sauce (a few years old now) 

![[Pasted image 20231127162256.png]]

ENA Express SSD big data flow instance types

![[Pasted image 20231127162342.png]]

Reduced P99 routing latencies by up to some big percentage...50%+?

David is AWS VPC OG dev

When the VPC feature launched AWS was one big flat network, basically, he says.

2013 VPC peering was released

Continuing need to scale pushed Transit Gateway development

### CapitalOne SVP Cloud and Networking

Will "something" from CapitalOne talking about how they live on public cloud juice

2015 

![[Pasted image 20231127162756.png]]

![[Pasted image 20231127162900.png]]
100k EC2 instances
200k Lambdas, maybe more

![[Pasted image 20231127162936.png]]

![[Pasted image 20231127163042.png]]

One common set of deployment and build tools across the enterprise, not for the faint of heart, but worth it.

Serverless is the way to go, long run.

Half of their applications are running on Fargate or other Serverless-ish things

![[Pasted image 20231127163201.png]]

![[Pasted image 20231127163232.png]]

They test network segmentation

![[Pasted image 20231127163253.png]]

Network address IP space is still a challenge. CIDR allocation still matters.
Private NAT gateways are the good answer.

![[Pasted image 20231127163428.png]]

Design for the "primarily distributed world that we now live in."

Back to you Dave.

Best customer testimonial so far, less pump piece and more practical value based content.

Transit gateways Inter-region peering, but no....

#### AWS cloud WAN

![[Pasted image 20231127163703.png]]

Maybe talk more about Terraform and CloudFormation

AWS Cloud WAN tunnel-less Connect

Umm, lots of words, no GRE overhead

Native BGP support, cool cool

More interoperability is good, clap clap clap from me.

#### Back to IP address management

#### CIDR samurai, Tina Morris

This person has to be a badass, by definition.

Amazon VPC IPAM Enhancements

![[Pasted image 20231127164129.png]]

Autonomous System Number import!

Free tier for IPAM

Cool, groovy, useful.

### IPV6 - The Future, obvi
#### IPV4 exhaustion

![[Pasted image 20231127164250.png]]

IPV6 contiguous blocks, makes sense

Gateway Load Balancer Support
BYO Firewall

Tina Morris is probably a genius engineer

I've been saying IP address management was a problem for....yeah, they just spent 20 minutes on that.

Anyway, let's go v6! It's been a long wait.

ARPANet history lesson, Load Balancer history, yada yada

2007 is when David joined AWS, Elastic Load Balancing team in 2013.

![[Pasted image 20231127164628.png]]

![[Pasted image 20231127164705.png]]

Anomaly detection with automatic target weight for grey failures in ALB Targets.

Generally available

![[Pasted image 20231127164751.png]]

Automatically weights out the failed node.

![[Pasted image 20231127165121.png]]

What if we could abstract away the networking? See above. Mesh networking to the next level, 

AWS VPC Lattice is generally available

Service network 

![[Pasted image 20231127165247.png]]

AWS Lattice is probably a sane way to do networking in a microservice-discovery environment. I like it.

Centuries of history including skytales

okay crypto, okay...yada yada crypto but pretending not to talk about crypto...skip skippity over this section into security....

Cryptocurrencies are embarrassing, face it.

Oh, cyber-crime Project Mad Pot

![[Pasted image 20231127165541.png]]

How to get banned by AI, if you have bad luck.

![[Pasted image 20231127165632.png]]

![[Pasted image 20231127165656.png]]

MadPot is realtime threat disruption at scale.

Perimeter threat detection vs internal threat detection
![[Pasted image 20231127165747.png]]

Rules based firewall at the network level

Blast radius control

![[Pasted image 20231127165833.png]]

BYOF

![[Pasted image 20231127165850.png]]

![[Pasted image 20231127165943.png]]

### Zero Trust Computing

![[Pasted image 20231127170027.png]]

AWS Verified Access ^

![[Pasted image 20231127170120.png]]

![[Pasted image 20231127170204.png]]
![[Pasted image 20231127170235.png]]
### recap
Printing press, load balancing, crypto, not sure what the through-thread is, but this was an information rich presentation that did not suck much, given how dry the material was.

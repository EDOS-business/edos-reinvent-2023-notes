## Cloud Operations for today, tomorrow, and beyond

###  Nandini Ramani

##### Vice President, Monitoring & Observability, AWS

> Over the years, AWS has innovated its cloud operations to support its own needs at scale and turned those capabilities on for you to solve your challenges in governance, compliance, observability, and operations as you build your applications in the cloud, on premises, in hybrid environments, and at the edge. Join this session to learn how AWS Cloud Operations is building for the future with automated governance and intelligent, efficient, and application-based operations that will power your growth and innovation. Hear how customers used AWS services to build their own cloud operating model for operational excellence that tore down silos and optimized costs.

Cloud operations Innovations talk

- Automating operations
- Improving performance and resilience
- Creating delightful customer experiences
- Improved developer experience

...and here comes the money...
### JP Morgan Chase & Co.

Is gigantic
##### Sanya Sridharan

- $15B tech spend
- First to invest in the light bulb
- First to public cloud
- 35k software engineers
- 600m+ lines of code
- High degree of variance
- Many langs
- Many environments, on-prem, cloud 
- heterogeneity and complexity magnify challenges
- Highly regulated industry
- Complex applications estate 

Engineer Platform and Integrated Experience (EPiX)
![[Pasted image 20231127114314.png]]

![[Pasted image 20231127114348.png]]

Observability as Code
Implemented as part of the developer experience

![[Pasted image 20231127114521.png]]

## Scaling Governance

### AWS Control Tower

![[Pasted image 20231127114818.png]]

![[Pasted image 20231127114913.png]]
![[Pasted image 20231127114926.png]]

^^ neat

![[Pasted image 20231127115012.png]]

![[Pasted image 20231127115049.png]]

#### You can't manage what you can't see
- Log everything
- Cloudwatch
- AWS eats their own dog food

#### Monitoring for compliance in AWS control tower configuration with Systems Manager

Also works on other clouds

AWS Cloud Operations helps you in hybrid and multicloud environments

CloudWatch data querying from multiple source, across clouds and other envirnonments.

Ingests custom data sources too!


![[Screenshot 2023-11-27 at 11.54.17 AM.png]]

Low code - no-code tools

AWS Systems Manager

![[Pasted image 20231127115522.png]]

Runbooks, you say? Interesting

"Log Insights" grouping


#### AWS Config 
Periodic recording released, instead of continuous

On Thursday Dr. Werner Vogels will share more

## Alexi from Disney

#### This guy is in on the Disney, full bore

![[Pasted image 20231127120250.png]]

How to scale across this diverse brand landscape, but in the cloud?

### Old Days were slow days


- weeks to set up an account? Really?
	- IAM accounts/roles/policies
	- Network and resource access
- They created a team to handle the "speed to delivery" problem with good back office tooling
	- Leveraged AWS tools like...
		- there is some stalling here, I want more detail
		- this is all set-up
- One-stop data shop, he says, Athena he says, visualization tools that AWS provides, he says, still no details.

Boss, can I get some details, please?

Base account set-up scaffolding includes access to the consolidated developer environments

![[Pasted image 20231127120702.png]]

Still no specific requirements, but there are some good ideas here, in terms of broad theory.

Segmenting of teams is bad, in terms of information sharing. They focused on creating a centralized community of good ideas for developers. 

Self-service functions seem to make the development teams more invested in the tools they use, which improves the tools.

Alexi obviously has built things, but he's not allowed to talk about them, or he chose not to.

Back to Nandini, and then 

## David Yanacek

### Lead AI Engineer and all around tech pogger

![[Pasted image 20231127121256.png]]

DevOps for building AWS tools like DynamoDB

This ain't it
![[Pasted image 20231127121438.png]]

Log Insights
![[Pasted image 20231127121455.png]]

this is. not better

#### Emergency Beacons

Filter logs

![[Pasted image 20231127121525.png]]

Now we have to figure out how to write a query.

![[Pasted image 20231127121611.png]]

Query Generator! neat

![[Pasted image 20231127121716.png]]

query bucketed by minute

Look at trends quickly

![[Pasted image 20231127121804.png]]

Non-technical people in shambles

It's AI, it's not AI, it's ML, but okay hype machine.

![[Pasted image 20231127121853.png]]
beam him up

Pattern matching grouping

![[Screenshot 2023-11-27 at 12.20.43 PM.png]]

Automatically finds anomalies, checkbox opt-in!

![[Pasted image 20231127122422.png]]

I bet they want a pretty penny for this feature

![[Pasted image 20231127122552.png]]

![[Pasted image 20231127122617.png]]

AWS Config Query

Sick demo David, you rock.
### thank you David Yanacek

Huge pitch on governance and policy, also interoperability with other systems. 

Interesting turn, I like it.


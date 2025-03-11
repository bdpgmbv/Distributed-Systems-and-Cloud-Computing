#### What is cloud computing ?

Quotes: Different opinions from tech leaders like Larry Ellison (Oracle) and Richard Stallman (Free Software Foundation) on what cloud computing is.
Main Point: Cloud computing is a buzzword with many definitions.

#### Software as a Service(SaaS)

Definition: SaaS is software provided over the internet, like Google Apps.
Benefits: Users save money and get easy access; providers find it easier to maintain and control.

#### Utility Computing 

Utility Computing is like renting computing resources (like processing power, memory, and storage) from a provider, just like you rent electricity or water from a utility company. Instead of buying and maintaining your own servers, you pay for what you use, when you need it.

##### Key Idea: Pay-as-You-Go
You only pay for the computing resources you actually use.
If you need more resources (like during a busy season), you can quickly get more.
If you need less, you can scale down and save money.

##### Examples of Utility Computing
Amazon EC2 (Elastic Compute Cloud): Lets you rent virtual machines (VMs) to run your software.
Microsoft Azure: Lets you run web applications and services in the cloud.
Google Cloud: Provides computing resources for businesses and developers.

##### How Does Utility Computing Work?
Imagine you’re running a website:
Instead of buying your own servers, you rent computing power from a provider like Amazon or Microsoft.
When your website gets more visitors, you can quickly get more resources to handle the traffic.
When traffic slows down, you can reduce the resources and pay less.

##### Types of Utility Computing
There are three main types, depending on what you need:

1. Infrastructure as a Service (IaaS)
What it is: You rent basic computing resources like virtual machines, storage, and networking.
Example: Amazon EC2 lets you rent virtual servers to run your applications.

2. Platform as a Service (PaaS)
What it is: You rent a platform to develop and run your applications. The provider manages the underlying infrastructure (like servers and storage).
Example: Microsoft Azure lets you build and deploy web applications without worrying about the hardware.

3. Software as a Service (SaaS)
What it is: You use software applications provided by a vendor over the internet.
Example: Google Apps (like Gmail and Google Docs) are SaaS applications.

##### Why is Utility Computing Useful?
Cost Savings: You don’t need to buy expensive hardware or pay for maintenance. You only pay for what you use.
Scalability: You can easily scale up or down based on your needs. For example:
If your website gets a sudden surge in traffic, you can quickly get more resources.
If traffic drops, you can reduce resources and save money.

Flexibility: You can choose the type of service (IaaS, PaaS, or SaaS) that fits your needs.

No Upfront Commitment: You don’t need to make a big investment upfront. You pay as you go.

##### Real-World Example: Animoto
What Happened: Animoto, a video creation service, saw a huge surge in demand when it went viral on Facebook.
How Utility Computing Helped: Animoto used Amazon EC2 to quickly scale from 50 servers to 3,500 servers in just 3 days to handle the traffic.
Result: Animoto didn’t need to buy thousands of servers upfront. They just rented what they needed, and when the demand dropped, they scaled back down.

##### Challenges of Utility Computing
Over-Provisioning vs Under-Provisioning:
Over-Provisioning: Buying too many resources and wasting money.
Under-Provisioning: Not having enough resources, leading to poor performance.
Utility Computing Solution: You can scale resources up or down as needed, avoiding both problems.

Performance Unpredictability:
Sometimes, the performance of cloud resources can vary.
Solution: Providers are improving virtualization and using technologies like flash memory to make performance more consistent.

Data Transfer Bottlenecks:
Transferring large amounts of data to and from the cloud can be slow.
Solution: Some companies physically send hard drives to the cloud provider (like FedEx-ing disks) to avoid slow internet transfers.

#### Amazon EC2
What it is: Amazon's Elastic Compute Cloud lets you rent virtual machines (VMs) to run your software.
How it works: You create a machine image (AMI), upload it, and configure it using Amazon's web service.

#### Utility computing - MS Azure
How to use: Develop your web program locally, then upload it to Azure

#### Spectrum of Abstractions 
Abstraction Levels: Different levels of cloud services, from low-level (Amazon EC2) to high-level (Azure).

#### Cloud Computing 
Combination: Cloud computing combines SaaS and PaaS (utility computing).
Analogy: Compares cloud computing to video on demand (SaaS) and electricity on demand (PaaS).

####  Significance of Cloud Computing
Benefits: Infinite resources, no upfront commitment, pay-as-you-go.

#### Economics of the Cloud
Cost Analysis: Discusses whether moving to the cloud saves money, considering factors like utilization and data transfer time

#### Should I Move Into A Cloud?
Cost Analysis: Repeats the cost comparison between cloud and datacenter.
Other Factors: Re-implementing programs and moving data into the cloud.

#### Adoption Challenges
Challenges: Lists issues like availability, data lock-in, and security.
Examples: Companies like Coghead and The Linkup faced problems when they shut down.
Survey Results: IT professionals are concerned about security, performance, and vendor lock-in when using cloud services.

#### Growth Challenges
Challenges: Data transfer bottlenecks, performance unpredictability, and scalable storage.
Solutions: Suggests improvements like better VM support and auto-scaling.

#### Policy and Business Challenge
Challenges: Reputation sharing and software licensing.
Examples: Open-source software is easier to use in the cloud, while proprietary software like Windows is offered per hour on EC2.

### Distributed Systems 

#### Loss of Reliability
Issues: Links can corrupt messages, routers can get overloaded.

Solution: Retransmission protocols.





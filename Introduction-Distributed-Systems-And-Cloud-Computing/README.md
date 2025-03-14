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

#### What about the Web?
Web Servers: Don’t keep track of clients; use cookies and databases for user info.

#### Web Servers and Transactions
Web Servers: Forget interactions immediately after they happen.
Transactions: Purchases are recorded in a database.

#### What about the Cloud?
Data Centers: Complex distributed systems with many servers, load balancing, and security policies.

#### Networks 
#### Classic view of network API
Steps: Get host name, IP address, create socket, and send data.
TCP vs UDP: TCP ensures data arrives in order; UDP does not.

#### Classic approach "broken" in many ways 
Problems: DNS, NAT, firewalls, DHCP, and caches can cause issues.

### Tunneling
#### Tunneling Analogy
Example: Compares tunneling a car through a railroad to tunneling data packets through a network.

#### Tunneling in Networks
Process: Shows how data packets are encapsulated and sent through a network.

### Example Microsoft VPN stack
#### What is a VPN?
A VPN (Virtual Private Network) is like a secure tunnel between your computer and a server (e.g., your office or a website). It keeps your data safe from hackers and lets you access private networks over the internet.

#### What is the Microsoft VPN Stack?
The Microsoft VPN Stack is a set of layers (like steps) that your data goes through when you use a VPN. Each layer has a specific job, like adding security or making sure the data reaches the right place. Think of it like packing a gift:
You wrap the gift (encrypt the data).
You put it in a box (add headers for routing).
You send it through a delivery service (the internet).

#### Layers in the Microsoft VPN Stack
Let’s go through each layer step by step, with an example to make it easier to understand.

1. Application Layer
What it does: This is where the data is created. For example, if you’re sending an email, the email content is created here.
Example: You type a message in your email app (like Outlook). This is the application layer.

2. TCP (Transmission Control Protocol)
What it does: TCP breaks the data into smaller pieces (called packets) and makes sure they arrive in the correct order. If a packet gets lost, TCP will resend it.
Example: Your email is split into smaller pieces, like pages in a book. TCP makes sure all the pages arrive and are in the right order.

3. IP (Internet Protocol)
What it does: IP adds the source and destination addresses to the packets, so they know where to go.
Example: Each packet gets a "to" and "from" address, like a letter going through the mail.

4. PPP (Point-to-Point Protocol)
What it does: PPP wraps the data in a format that can be sent over the internet. It’s like putting your letter in an envelope.
Example: Your email packets are wrapped in a secure envelope so they can travel safely.

5. L2TP (Layer 2 Tunneling Protocol)
What it does: L2TP creates a tunnel for the data to travel through. This tunnel hides your data from outsiders.
Example: Imagine your envelope is placed inside a secure, invisible tube that goes straight to the recipient. No one can see or touch it.

6. UDP (User Datagram Protocol)
What it does: UDP sends the data quickly, but it doesn’t guarantee delivery. It’s faster than TCP but less reliable.
Example: The secure tube sends your envelope quickly, but if something goes wrong, it won’t resend it. This is fine for things like video calls, where speed is more important than perfection.

7. IPsec (Internet Protocol Security)
What it does: IPsec adds encryption to the data, so even if someone intercepts it, they can’t read it.
Example: Your envelope is locked with a secret code. Only the recipient has the key to open it.

8. PPPoE (PPP over Ethernet)
What it does: PPPoE connects your computer to the internet using Ethernet (like a wired connection). It wraps the data again so it can travel over the internet.
Example: The locked envelope is placed inside another envelope that’s designed for internet delivery.

9. Ethernet
What it does: Ethernet is the final step where the data is sent over the internet using cables or Wi-Fi.
Example: The envelope is handed to the postman (the internet), who delivers it to the recipient.

#### How It Works Together: A Real-Life Example
Let’s say you’re working from home and need to access your company’s private network:
* Application Layer: You open a file on your company’s server.
* TCP: The file is split into packets, and TCP ensures they all arrive correctly.
* IP: Each packet gets an address so it knows where to go.
* PPP: The packets are wrapped in a secure format.
* L2TP: A secure tunnel is created between your computer and the company’s server.
* UDP: The packets are sent quickly through the tunnel.
* IPsec: The packets are encrypted so no one can read them.
* PPPoE: The encrypted packets are wrapped again for internet delivery.
* Ethernet: The packets are sent over the internet to the company’s server.

#### Why This Matters
1. Security: Your data is encrypted and hidden from hackers.
2. Privacy: No one can see what you’re sending or receiving.
3. Access: You can securely access private networks, like your office, from anywhere.

### END-TO-END ARGUMENT
#### What is the End-to-End Argument?
The End-to-End Argument is a design principle for building systems, especially networks like the internet. It says that certain functions (like reliability, security, or error-checking) should be handled by the endpoints (the sender and receiver) rather than by the network itself (the routers and links in between).

#### Why is it Called "End-to-End"?
End-to-End means from the sender to the receiver. The idea is that the two endpoints (the sender and receiver) are responsible for making sure the data is correct, secure, and delivered properly.
The network in the middle (routers, links, etc.) should focus on speed and efficiency, not on fixing errors or ensuring reliability.

#### Example to Understand It Better
Imagine you’re sending a letter to a friend:

#### End-to-End Approach: 
You write the letter, put it in an envelope, and your friend opens it and reads it. If something goes wrong (like the letter gets lost or damaged), you and your friend handle the problem (e.g., you send the letter again).
Network Approach: The post office (the network) tries to fix every possible problem along the way (e.g., if the envelope tears, they repair it). But this slows things down and adds complexity.
The End-to-End Argument says it’s better to let the endpoints (you and your friend) handle problems, while the network (post office) focuses on delivering the letter as fast as possible.

#### How Does This Apply to the Internet?
In the internet:
Endpoints: Your computer (sender) and the server (receiver).
Network: Routers, cables, and other devices that pass data between your computer and the server.

#### The End-to-End Argument says:
The network should focus on delivering packets as quickly as possible.
The endpoints should handle reliability, security, and error-checking.

#### Why is This Important?
Efficiency: If the network tries to handle everything (like fixing errors or ensuring security), it becomes slow and complicated.
Flexibility: Endpoints can decide how to handle problems based on their needs. For example:
If you’re sending a file, you might want to check for errors and retransmit if something goes wrong.
If you’re streaming a video, you might just skip a corrupted packet to keep the video playing smoothly.
Simplicity: The network doesn’t need to know about every application’s needs. It just delivers packets.

#### Example: File Transfer
End-to-End Approach: When you send a file, your computer breaks it into packets and sends them. The server checks if all packets arrived correctly. If some are missing, the server asks your computer to resend them.
Network Approach: Every router along the way checks for errors and tries to fix them. This slows down the transfer and adds unnecessary complexity.
The End-to-End Argument says the first approach is better.

#### When Should the Network Do More?
Sometimes, the network should handle certain tasks:
Performance Gains: For example, on a slow or unreliable link (like Wi-Fi), the network might retransmit lost packets to improve speed.
Security: In some cases, the network might encrypt data to protect it from hackers.
Special Cases: Tasks like routing (deciding the best path for data) or billing (charging users for data usage) must be done by the network.

#### Key Takeaways
Endpoints Handle the Hard Stuff: Reliability, security, and error-checking should be done by the sender and receiver.
Network Focuses on Speed: The network should deliver data as fast as possible without worrying about fixing errors.
Flexibility and Simplicity: This approach makes the system simpler and more adaptable to different needs.

#### Real-World Example: Email
End-to-End Approach: When you send an email, your email client (like Gmail) ensures the email is delivered correctly. If the email doesn’t reach the recipient, your email client will retry or notify you.

Network Approach: If the network tried to ensure every email was delivered, it would slow down all internet traffic and make the system overly complex.

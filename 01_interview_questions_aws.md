## Changes
*Modified answers to  questions 1,2,3,5,6,8,9,12,13*
---
## What is AWS ?

### Explanation

Amazon Web Services (AWS) is the world’s most comprehensive and broadly adopted cloud, offering over 200 fully featured services from data centers globally. Millions of customers—including the fastest-growing startups, largest enterprises, and leading government agencies—are using AWS to lower costs, become more agile, and innovate faster.
It provides those services as :

### Infrastructure as a Service (IaaS)

- **Infrastructure as a Service (IaaS)** is a self-service model for managing remote data center infrastructures. AWS offers IaaS in the form of data centers.
  - **Example** : Amazon Web Services, Microsoft Azure, and Google Compute Engine

### Platform as a Service (PaaS)

- **Platform as a Service (PaaS)** allows organizations to build, run and manage applications without the IT infrastructure. This makes it easier and faster to develop, test and deploy applications.
  - **Example** : AWS Elastic Beanstalk, Google App Engine,

### Software as a Service (SaaS)

- **Software as a service (SaaS)** replaces the traditional on-device software with software that is licensed on a subscription basis. It is centrally hosted in the cloud. A good example is Salesforce.com.
  - **Example** : Gmail, Slack, and Microsoft Office 365

---

## What are the important/most common components/services of AWS that you have used?

### Explanation

AWS provides over 200 fully featured services from data centers to millions of customers globally.
Some of the AWS services that I have used are as follows

- **Simple Storage Service (S3) :** Amazon S3, at its core, facilitates object storage, providing leading scalability, data availability, security, and performance. Businesses of vast sizes can leverage S3 for storage and protect large sums of data for various use cases, such as websites, applications, backup, and more.
- **Elastic Compute Cloud (EC2) :** Elastic Compute Cloud is a web service that provides resizable compute capacity in the cloud.
- **Elastic Beanstalk :** It provides services to deploy a different application which is available in different platforms or languages like java, nodejs etc.
- **Relational Database Service (Amazon RDS) :** is a collection of managed services that makes it simple to set up, operate, and scale databases in the cloud. Choose from seven popular engines — Amazon Aurora with MySQL compatibility, Amazon Aurora with PostgreSQL compatibility, MySQL, MariaDB, PostgreSQL, Oracle, and SQL Server — and deploy on-premises with Amazon RDS on AWS Outposts.

---

## Explain the Key-pairs in detail

### Explanation

A key pair, consisting of a public key and a private key, is a set of security credentials that you use to prove your identity when connecting to an Amazon EC2 instance.
Amazon EC2 stores the public key on your instance, and you store the private key.
Anyone who possesses your private key can connect to your instances, so it's important that you store your private key in a secure place.

When you launch an instance, you can specify a key pair. If you plan to connect to the instance using SSH, you must specify a key pair. You can choose an existing key pair or create a new one.

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html

---

## Explain the term “Cross Region Replication” (CRR)

### Explanation

Amazon S3 supports cross-region replication (CRR), a feature that automatically replicates data across AWS regions.
Replication enables automatic, asynchronous copying of objects across Amazon S3 buckets.
With cross-region replication, every object uploaded to an S3 bucket is automatically replicated to a destination bucket in a different AWS region that you choose.
For example, you can use cross-region replication to provide lower-latency data access in different geographic regions.
Cross-region replication can also help if you have a compliance requirement to store copies of data hundreds of miles apart. There is no additional charge for using cross-region replication.
You pay Amazon S3’s usual charges for storage, requests, and inter-region data transfer for the replicated copy of data.
https://docs.aws.amazon.com/AmazonS3/latest/userguide/replication.html

---

## What do we understand by Regions and Availability Zones(Global Infrastructure) in AWS

### Explanation

**Availability Zone (AZ) :** An Availability Zone (AZ) is one or more discrete data centers with redundant power, networking, and connectivity in an AWS Region. AZs give customers the ability to operate production applications and databases that are more highly available, fault tolerant, and scalable than would be possible from a single data center. All AZs in an AWS Region are interconnected with high-bandwidth, low-latency networking, over fully redundant, dedicated metro fiber providing high-throughput, low-latency networking between AZs. All traffic between AZs is encrypted. The network performance is sufficient to accomplish synchronous replication between AZs.

**Regions :** AWS has the concept of a Region, which is a physical location around the world where we cluster data centers. We call each group of logical data centers an Availability Zone. Each AWS Region consists of a minimum of three, isolated, and physically separate AZs within a geographic area. Unlike other cloud providers, who often define a region as a single data center, the multiple AZ design of every AWS Region offers advantages for customers. Each AZ has independent power, cooling, and physical security and is connected via redundant, ultra-low-latency networks. AWS customers focused on high availability can design their applications to run in multiple AZs to achieve even greater fault-tolerance. AWS infrastructure Regions meet the highest levels of security, compliance, and data protection.

**Edge Locations :** Edge locations are AWS data centers designed to deliver services with the lowest latency possible. Amazon has dozens of these data centers spread across the world. They’re closer to users than Regions or Availability Zones, often in major cities, so responses can be fast and snappy.

https://aws.amazon.com/about-aws/global-infrastructure/regions_az/

## Define Auto Scaling and list some of its advantages

### Explanation

AWS Auto Scaling monitors your applications and automatically adjusts capacity to maintain steady, predictable performance at the lowest possible cost. Using AWS Auto Scaling, it’s easy to setup application scaling for multiple resources across multiple services in minutes. The service provides a simple, powerful user interface that lets you build scaling plans for resources including Amazon EC2 instances. AWS Auto Scaling makes scaling simple with recommendations that allow you to optimize performance, costs, or balance between them.
Advantages of Auto Scaling
**SETUP SCALING QUICKLY**
- AWS Auto Scaling lets you set target utilization levels for multiple resources in a single, intuitive interface. You can quickly see the average utilization of all of your scalable resources without having to navigate to other consoles. For example, if your application uses Amazon EC2 and Amazon DynamoDB, you can use AWS Auto Scaling to manage resource provisioning for all of the EC2 Auto Scaling groups and database tables in your application.
**MAKE SMART SCALING DECISIONS**
- AWS Auto Scaling lets you build scaling plans that automate how groups of different resources respond to changes in demand. You can optimize availability, costs, or a balance of both.
**AUTOMATICALLY MAINTAIN PERFORMANCE**
- Using AWS Auto Scaling, you maintain optimal application performance and availability, even when workloads are periodic, unpredictable, or continuously changing. AWS Auto Scaling continually monitors your applications to make sure that they are operating at your desired performance levels. When demand spikes, AWS Auto Scaling automatically increases the capacity of constrained resources so you maintain a high quality of service.
**PAY ONLY FOR WHAT YOU NEED**
- AWS Auto Scaling can help you optimize your utilization and cost efficiencies when consuming AWS services so you only pay for the resources you actually need. When demand drops, AWS Auto Scaling will automatically remove any excess resource capacity so you avoid overspending. AWS Auto Scaling is free to use, and allows you to optimize the costs of your AWS environment.
https://aws.amazon.com/autoscaling/
---
## What is an AMI?
### Explanation
AMI stands for Amazon Machine Image.It is a virtual image used to create a virtual machine within an EC2 instance.
An Amazon Machine Image (AMI) is a supported and maintained image provided by AWS that provides the information required to launch an instance. You must specify an AMI when you launch an instance. You can launch multiple instances from a single AMI when you require multiple instances with the same configuration. You can use different AMIs to launch instances when you require instances with different configurations.

An AMI includes the following:

- One or more Amazon Elastic Block Store (Amazon EBS) snapshots, or, for instance-store-backed AMIs, a template for the root volume of the instance (for example, an operating system, an application server, and applications).

- Launch permissions that control which AWS accounts can use the AMI to launch instances.

- A block device mapping that specifies the volumes to attach to the instance when it's launched.

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AMIs.html
---
## Why do you use policies in AWS and how many types of policies are in AWS?

### Explanation
The policy is an object which is associated with a resource that defines the permissions.AWS evaluate these policies when the user makes a request.Permissions in the policy determine whether to allow or deny an action.Policies are stored in the form of JSON documents.
The following policy types, listed in order from most frequently used to less frequently used, are available for use in AWS. 

- **Identity-based policies –** Attach managed and inline policies to IAM identities (users, groups to which users belong, or roles). Identity-based policies grant permissions to an identity.

- **Resource-based policies –** Attach inline policies to resources. The most common examples of resource-based policies are Amazon S3 bucket policies and IAM role trust policies. Resource-based policies grant permissions to the principal that is specified in the policy. Principals can be in the same account as the resource or in other accounts.

- **Permissions boundaries –** Use a managed policy as the permissions boundary for an IAM entity (user or role). That policy defines the maximum permissions that the identity-based policies can grant to an entity, but does not grant permissions. Permissions boundaries do not define the maximum permissions that a resource-based policy can grant to an entity.

- **Organizations SCPs –** Use an AWS Organizations service control policy (SCP) to define the maximum permissions for account members of an organization or organizational unit (OU). SCPs limit permissions that identity-based policies or resource-based policies grant to entities (users or roles) within the account, but do not grant permissions.

- **Access control lists (ACLs) –** Use ACLs to control which principals in other accounts can access the resource to which the ACL is attached. ACLs are similar to resource-based policies, although they are the only policy type that does not use the JSON policy document structure. ACLs are cross-account permissions policies that grant permissions to the specified principal. ACLs cannot grant permissions to entities within the same account.

- **Session policies –** Pass advanced session policies when you use the AWS CLI or AWS API to assume a role or a federated user. Session policies limit the permissions that the role or user's identity-based policies grant to the session. Session policies limit permissions for a created session, but do not grant permissions. For more information, see Session Policies.

https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html

---
## S3 Storage Classes
### Explanation
Each object in Amazon S3 has a storage class associated with it. For example, if you list the objects in an S3 bucket, the console shows the storage class for all the objects in the list. Amazon S3 offers a range of storage classes for the objects that you store. You choose a class depending on your use case scenario and performance access requirements. All of these storage classes offer high durability.

### Storage classes for frequently accessed objects
For performance-sensitive use cases (those that require millisecond access time) and frequently accessed data, Amazon S3 provides the following storage classes:

- **S3 Standard –** The default storage class. If you don't specify the storage class when you upload an object, Amazon S3 assigns the S3 Standard storage class.

- **Reduced Redundancy –** The Reduced Redundancy Storage (RRS) storage class is designed for noncritical, reproducible data that can be stored with less redundancy than the S3 Standard storage class.

### Storage class for automatically optimizing data with changing or unknown access patterns
- **S3 Intelligent-Tiering** is an Amazon S3 storage class that's designed to optimize storage costs by automatically moving data to the most cost-effective access tier, without performance impact or operational overhead. S3 Intelligent-Tiering is the only cloud storage class that delivers automatic cost savings by moving data on a granular object level between access tiers when access patterns change. S3 Intelligent-Tiering is the ideal storage class when you want to optimize storage costs for data that has unknown or changing access patterns. 

### Storage classes for infrequently accessed objects
- The **S3 Standard-IA** and **S3 One Zone-IA** storage classes are designed for long-lived and infrequently accessed data. *(IA stands for infrequent access.)* S3 Standard-IA and S3 One Zone-IA objects are available for millisecond access (similar to the S3 Standard storage class). Amazon S3 charges a retrieval fee for these objects, so they are most suitable for infrequently accessed data.

### Storage classes for archiving objects
- The **S3 Glacier Instant Retrieval, S3 Glacier Flexible Retrieval, and S3 Glacier Deep Archive** storage classes are designed for low-cost data archiving. These storage classes offer the same durability and resiliency as the S3 Standard and S3 Standard-IA storage classes

https://docs.aws.amazon.com/AmazonS3/latest/userguide/storage-class-intro.html
---


# Storage Gateway

**VERY POPULAR EXAM TOPIC**

## Storage Gateway
AWS Storage Gateway is a service that connects an on-premisess software appliance with cloud-based storage to provide seamless and secure integration between an organization's on-premises IT environment and AWS's storage infrastructure. The service enables you to securely store data to the AWS cloud for scalable and cost-effective storage.

AWS Storage Gateway's software appliance is available for download as a virtual machine (VM) image that you install on host in your datacenter. Storage Gateway supports either VMware ESXi or Microsoft Hyper-V. Once you've installed your gateway and associated it with your AWS account through the activation process, you can use the AWS Management Console to create the storage gateway option that is right for you.

## Four type of Storage Gateway
* File Gateway (NFS) - Store flat files in S3, such as PDF, images, etc.
* Volume Gateway (iSCSI) - Block based storeage, could be a virtual harddisk that your VM is running on, not for flat files. This type consists of:
  * Stored Volumes - This is where you store the entire copy of your data set on-site/on-premise
  * Cached Volumes - Store the most recently accessed only
* Tape Gateway (VTL) - Back up and archiving solution that allows you to create virtual tape to S3, and you can send that virtual tape to Glacier

### File Gateway (Flat file) - More on
Files are stored as objects in your S3 buckets, accessed through a Network File System (NFS) mount point. Ownership, permissions, and timestamps are durably stored in S3 in the user-metadata of the object associated with the file. Once objects are transferred to S3, they can be managed as native S3 objects, and bucket policies such as versioning, lifestyle management, and cross-region replication apply directly to objects in your bucket.
(Unlikely show in the exam)

### Volume Gateway (Block-based storage) - More on
The volume interface presents your applications with disk volumes using the iSCSI block protocol. Block-based storage that you can store Operating System, application such as SQL server, run databases from it. So, think of this as **Virtual Hardisk**

Data written to these volumes can be asynchronously backed up as point-in-time snapshots of your volumes, and stored in the cloud as Amazon EBS (Elastic Block Store) snapshots. EBS is a virtual hardisk, storage that will be attached to EC2 instances.

Snapshots are incremental backups that capture only changed blocks. All snapshot storage is also compressed to minimize your storage charges.

*NOTE*: Volume Gateway is basically a Virtual Harddisk that is ready to be used by other AWS instances.

There are 2 different types of **Volume Gateway**
* **Stored Volumes** - Stored volumes let you store your primary data locally, while asynchronously backing up that data to AWS. Stored volumes provide your on-premises applications with low-latency access to their entire datasets, while providing durable, off-site backups. You can create storage volumes and mount them as iSCSI devices from your on-promises application servers. Data written to your stored volumes is stored on your on-premises storage hardware. This data is asynchronously backed up to Amazon Simple Storage Service (Amazon S3) in the form of Amazon Elastic Block Store (Amazon EBS) snapshots. 1 GB - 16 TB in size for Stored Volumes.
* **Cached Volumes** - Cached volumes let you use Amazon Simple Storage Service (Amazon S3) as your primary data storage while retaining frequently accessed data locally in your storage gateway. Cached volumes minimize the need to scale your on-premises storage infrastructure, while still providing your applications with low-latency access to their frequently accessed data. You can create storage volumes up to 32 TiB in size and attach ot them as iSCSI devices from your on-premises application servers. Your gateway stores data that you write to these volumes in Amazon S3 and retains recently read data in your on-premises storage gateway's cached an upload buffer storage. 1 GB - 32 TB in size for Cached Volumes. (Basically, everytime you write data, it will be stored in S3, while everytime you read data, it will be stored in on-premises Cache Storage.)

### Tape Gateway - More on
Tape Gateway offers a durable, cost-effective solution to archive your data in the AWS cloud.


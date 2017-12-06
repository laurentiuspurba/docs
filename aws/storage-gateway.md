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

### File Gateway - More on
Files are stored as objects in your S3 buckets, accessed through a Network File System (NFS) mount point. Ownership, permissions, and timestamps are durably stored in S3 in the user-metadata of the object associated with the file. Once objects are transferred to S3, they can be managed as native S3 objects, and bucket policies such as versioning, lifestyle management, and cross-region replication apply directly to objects in your bucket.
(Unlikely show in the exam)

### Volume Gateway - More on
The volume interface presents your applications with disk volumes using the iSCSI block protocol.

Data written to these volumes can be asynchronously backed up as point-in-time snapshots of your volumes, and stored in the cloud as Amazon EBS snapshots.

Snapshots are incremental backups that capture only changed blocks. All snapshot storage is also compressed to minimize your storage charges.

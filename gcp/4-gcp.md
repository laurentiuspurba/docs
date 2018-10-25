# Core Storage

Either for structured, un-structed, transactional and relational data.

They are few options, they are:
* Cloud Storage
* Cloud SQL
* Cloud Spanner
* Cloud Data Store
* Google Big Table

## Cloud Storage
![Alt text](images/gcpcloudstorage.png?raw=true "GCP Cloud Storage")

Object storage:
* is not the same as file storage in which you manage your data as hierarchy of folders.
* is not the same as block storage in which your operating system manages your data as chunck of disks
* means you save your storage here; the storage addresses us with unique key. Often these unique keys are in the form of URLs which means object storage interacts nicely with web technologies

**Cloud Storage** works just like object storage plus it is fully managed, scalable service with high durability and availability. That means you don't need to provision capacity ahead of time.

Cloud Storage usage:
* Serving website content
* Storing data for archival and disaster recovery
* Distributing large data object to your end user via direct download

**ACHTUNG** Cloud Storage is not a filesystem!!!

Cloud storage characteristics:
* Each object in cloud storage has a URL
* Each field is like a file (informally) in a lot of ways
* Do not use cloud storage as root of your file system in linux
* Comprise of buckets; you create, configure and use to hold your storage object
* This storage object is mutable which means you cannot edit it in place, but instead you have to create a new version
* Cloud storage always encrypts your data in the server side before it is written to disk
* By default, data in transit is encrypted via https
* There is a service to transfer your large amount of data to Cloud storage

![Alt text](images/cloudstoragetableinfo.png?raw=true "GCP Cloud Storage Info")

# Cloud SQL
![Alt text](images/cloudsql.png?raw=true "Cloud SQL")

Cloud SQL is a fully manage RDBMS
As of now it offers:
* MySQL
* PostgreSQL - beta as of Mon Oct 29, 2018

Benefits running Cloud SQL instead of SQL on VM instance:
* Automatic replication
* Managed backups: on-demand or scheduled backups
* Scale vertically (read and write) by changing machine type
* Scale horizontally (read) via read replicas
* Google security includes
  * Network firewalls
  * Encrypted
* Accessible by other GCP services and even external services

![Alt text](images/cloudsqlcanbeusedwithothergcpservices.png?raw=true "Cloud SQL used with other GCP Services")


# Cloud Spanner
![Alt text](images/cloudspanner.png?raw=true "Cloud Spanner")

If Cloud SQL does not fit your requirements because you need **horizontal** scalability, consider using **Cloud Spanner**

It offers:
* transactional strong consistency at global scale
* managed instances with high availability
* schemas, SQL, and automatic synchronize replication for HA
* petabyte of capacity

Consider using cloud spanner if:
* Outgrown any relational database
* Sharding your databases for throughput high performance
* Need transactional consistency
* Global data and strong consistency
* Just to consolidate your database

Natural use case includes:
* Financial application
* Inventory application

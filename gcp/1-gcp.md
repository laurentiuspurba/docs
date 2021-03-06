# Google Cloud Platform - GCP

It provides 4 main kind of services:
* Compute
* Storage
* Big data
* Machine Learning

## What is Cloud computing?
It is:
* On-deman self-service - No human intervention needed to get resources
* Broad network access - Access from anywhere
* Resouce pooling - Provider shares resources to customer
* Rapid elasticity - Get more resources quickly as needed
* Measure service - Pay only what you consume

## GCP architecture
![Alt text](images/Screen%20Shot%202018-07-10%20at%209.30.31%20PM.png?raw=true "GCP Architecture")

## Region and Zone
GCP is organized into regions and zones.
* zones - europe-west2-a, europe-west2-b, europe-west2-c
* region- europe-west2
* multi region -europe

As of now, GCP has 15 regions around the world.

### Compute Services
Consists of:
* Compute Engine
* Kubernetes Engine
* App Engine
* Cloud Functions

### Storage Services
Consists of:
* Big Table
* Cloud Storage
* Cloud SQL
* Cloud Spanner
* Cloud Datastore

### Big Data Services
Consists of:
* Big Query
* Pub/Sub
* Dataflow
* Dataproc
* Datalab
### Machine Learning Services
Conists of:
* Natural Language API
* Vision API
* Machine Learning
* Speech API
* Translate API

## Multi-layered security approach
| Layer   | Notable security measures (among others)  |
|---|---|
| Operational security | Intrusion detection system; techniques to reduce insider risk; employee U2F use; software development practices |
| Internet communication | Google Front End; designed-in Denial of Service protection |
| Storage services  | Encryption at rest |
| User identity | Central identity service with support of U2F |
| Service deployment | Encryption of inter-service communication |
| Hardware infrastructure | Hardware design provenance; secure boot stack; premises security |

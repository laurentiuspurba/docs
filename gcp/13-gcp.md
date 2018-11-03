# Development in the Cloud

* Cloud Source Repositories is fully featured Git repositories hosted on GCP
* Cloud Functions (Beta) creates single-purpose functions that respond to events without a server or runtime:
  * Ex. image upload processing; written in Javascript; execute in managed NodeJS environment on GCP (can trigger in on events in Cloud Storage, Cloud PubSub or http call)

# Deployment: Infrastructure as code

Deployment manager is an infrastructure management service that automates the creation and management of a Google Cloud Platform resources for you. It provides repeatable deployments.
To use it, you have to create a **template file**, either in yaml or python. This template describes your environment and use Deployment Manager to create resources.

Important tip: You can store and version control your deployment manager templates in Cloud Source Repositories.

# Monitoring
 
Monitoring lets you figure out whether the changes you made are good or bad.

## Stackdriver
It is for:
* Monitoring
* Logging
* Debug
* Error reporting
* Trace

### Core component of Stackdriver
![Alt text](images/corecomponentsofstackdriver.png?raw=true "Stackdriver core comps")

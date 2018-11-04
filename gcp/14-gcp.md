# Google Cloud Big Data

Google Cloud Big Data solutions are designed to help you to transform your businesses and user experiences with meaningful data insight.
It is called **Integrated serveless platform**.

**Integrated serverless platform**
![Alt text](images/bigdataserverlessplatform.png?raw=true "Integrated serverless platform")

## Cloud Dataproc
Cloud Dataproc is managed by Hadoop
* It is great, if you have a known data size
* Fast, easy, managed way to run Hadoop and Spark/Hive/Pig on GCP
* Create cluster in 90 seconds or less on average
* Scale clusters up and down even when jobs are running

Why use Cloud Dataproc?
* Easily migrate on-premises Hadoop jobs to the cloud
* Save money with preemptible instances
* Use Spark Machine Learning Libraries (MLlib) to run classification algorithms

## Cloud Dataflow

When you have data in real time or it's of unpredicatable size or rate, you need **Cloud Dataflow**.

Cloud Dataflow offers managed data pipeline
* Fully automate; serverless
* Processes data using Compute Engine instances
  * Clusters are sized for you
  * Automated scaling, no instance provisioning required
* It's both unified programming model and managed service
* Lets you develop and execute a big range of data processing patterns
* Extract, to Transform, and Load (ETL) batch computation and continuous computation
* Build pipelines for batch and streaming data
* Write code once and get batch and streaming
  * Transform-based programming model

Example

![Alt text](images/clouddataflowexample.png?raw=true "Cloud Dataflow example")

Why use Cloud Dataflow?
* ETL (Extract, Transform, Load) pipelines to move, filter, enrich, and shape data
* Data analysis: batch computation or continuous computation using streaming
* Orchestration: create pipelines that coordinate services, including external services
* Integrates with GCP services like Cloud Storage, Cloud Pub/Sub, BigQuery, and Bigtable
  * Open sourc Java and Python SDKs
  
## Cloud BigQuery
Suppose, instead of a dynamic pipeline, your data needs to run more in the way of exploring a vast sea of data. You want to do ad hoc SQL queries on a massive data set. That's what BigQuery is for

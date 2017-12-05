# S3-Security and Encryption

## Securing your bucket
* By default, all newly created buckets are PRIVATE
* You can setup access controll to your buckets using:
* * Bucket Policies - Permission is applied to the entire bucket
* * Access Control Lists - Can be drilled down to individual objects
* S3 buckets can be configured to create access logs which log all requests made to the S3 bucket. This can be done to another bucket. (Or even another AWS account - cross account access)

## Encryption
Four S3 encryption methods:
* adf

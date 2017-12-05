# S3-Security and Encryption

## Securing your bucket
* By default, all newly created buckets are PRIVATE
* You can setup access controll to your buckets using:
* * Bucket Policies - Permission is applied to the entire bucket
* * Access Control Lists - Can be drilled down to individual objects
* S3 buckets can be configured to create access logs which log all requests made to the S3 bucket. This can be done to another bucket. (Or even another AWS account - cross account access)

## Encryption
Two type of encryption:
* In Transit - When you are sending data from and/to your bucket:
* * SSL/TLS
* At Rest: They are 4 different methods:
* * Server Side encryption: They are 3 different types:
* * * S3 Managed Keys - **SSE-S3** - Each object is encrypted with unique key, employing strong multifactor encryption; as additional safeguard, AWS encrypts the key itself with the master key, and reqularly rotate that master key. (AES256)
* * * AWS Key Management Service, Managed Keys - **SSE-KMS** - Basically, it is Key Management Service. It is similar to **SSE-S3**, but it comes with few additional benefits, as well as additional charges for using it. There is separate permission to use *envelope keys*, which is a key that protects data encryption key that provides added protection against un-authorized to your object in S3. The other advantage is audit trail. You can manage to create key yourself or use default one.
* * * Server Side Encryption With Customer Provided Keys - **SSE-C**
* * Client-side encryption

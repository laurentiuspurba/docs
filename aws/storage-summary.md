# S3 - Exam Tips for S3 101
* Remember that S3 is object based ie. it allows you to upload files.
  * Not for OS or DB.
* Files can be from 0 Bytes to 5TB.
* There is unlimited storage.
* Files are stored in buckets.
* S3 is a universal namespace, that is, names must be unique globally.
  * Ex. bucket name: https://s3-eu-west-1.amazonaws.com/whatever
* Read after Write consitency for PUTS of new Objects
* Eventual Consitency for overwrite PUTS and DELETES (can take some time to propagate)

## Storage Tiers/Classes
* S3 Standard: 99.99% availability, 99.999999999% durability, stored redudantly acros multiple devices in multiple facilities, and is designed to sustain the loss of 2 facilities concurently.
* S3 - IA: (Infrequently Access): For data that is access less frequently, but requires rapid access when needed. Lower fee than S3, but you are charge retrieval fee.

# CloudFront (CDN)

## What is CloudFront (CDN)
A content delivery network (CDN) is a system of distributed serves (network) that deliver webpages and other web content to a user based on the geographic locations of the user, the origin of the webpage and a content delivery server.

## Key Terminology
* Edge Location - This is the location where content will be cached. (This is separte to an AWS Region/Availability Zone - AZ)
* Origin - This is the origin of all the files that the CDN will distribute. This can be either S3 Bucket, an EC2 Instance, an Elastic Load Balancer or Route53
* Distribution - This is the name given the CDN which consists of a collection of Edge Locations

So, Amazon CloudFront can be used to delivery your entire website, including dynamic, static, streaming, and interactive content using a global network of edge locations. Requests for your content are automatically routed to the nearest edge location, so content is delivered with the best possible performance.

Amazon CloudFront is optimized to work with other Amazon Web Services, like Amazon Simple Storage Service (Amazon S3), Amazon Elastic Compute Cloud (Amazon EC2), Amazon Elastic Load Balancing, and Amazon Route53. Amazon CloudFront also works seamlessly with any non-AWS origin server, which stores the original, definitive versions of your files.

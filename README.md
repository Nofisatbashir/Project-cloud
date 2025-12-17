## AWS S3 Static Website Hosting
This project demonstrates how to host a static website using Amazon S3.
The task involved modifying an index.html file, creating and configuring an S3 bucket, uploading the file, enabling static website hosting, and generating a public endpoint.
## Objective
Create an S3 bucket in AWS
Upload a modified index.html file
Configure the bucket for static website hosting
Make the website publicly accessible
Generate and test the website endpoint
## Prerequisites
AWS account

Access to AWS Management Console

Modified index.html file
## Architecture Overview
Amazon S3 → Object storage

S3 Static Website Hosting → Serves content over HTTP

Bucket Policy → Controls public access
## Implementation Steps
1. Create an S3 Bucket
Navigate to AWS Console → S3
Click Create bucket
Bucket name: oyin-static-site
Region: eu-north-1
Disable Block all public access
Create the bucket
2. Upload the Website File
Open the bucket → Objects
Click Upload
Upload index.html
3. Enable Static Website Hosting
Go to Properties
Enable Static website hosting
Index document: index.html
## Website Endpoint
https://oyin-static-site.s3.eu-north-1.amazonaws.com/index.html
## Testing
Open the endpoint in a browser

Confirm the index.html page loads successfully
<img width="1118" height="661" alt="my web snip" src="https://github.com/user-attachments/assets/974b982a-82e5-4a60-a7d9-5a43cb5fedde" />

## Challenges Encountered and Resolution
Public access errors:

Resolved by disabling Block Public Access at the bucket level and applying the correct bucket policy.

AWS console “Unexpected error” messages:

<img width="1362" height="660" alt="error 1" src="https://github.com/user-attachments/assets/43b587b8-856c-4c37-8541-90b143947d85" />




Identified as permission conflicts caused by public access restrictions.
## Conclusion
This project successfully demonstrated how to host a static website using Amazon S3. By leveraging S3 static website hosting, the website was deployed without the need for servers, making the solution scalable, cost-effective, and easy to manage. 



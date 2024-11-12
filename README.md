<h1>Securing-Content-Delivery-with-Amazon-CloudFront-and-Origin-Access-Control-OAC</h1>

<h2>Description</h2>
This project utilizes Amazon CloudFront, a content delivery network (CDN), integrated with Amazon S3 and secured through Origin Access Control (OAC). The goal is to deliver content to users with high performance and low latency while maintaining strict security controls to restrict direct access to the origin (S3 bucket). OAC ensures that only CloudFront can access the S3 bucket, adding a layer of protection against unauthorized access. This configuration helps websites, applications, or media streaming platforms deliver secure, scalable, and fast content globally.
<br />

<h2>Deliverables: </h2>

- <b>Configured S3 bucket with enforced encryption standards.</b> 
- <b>Documentation of setup, policies, and audit logs.</b>
- <b>Optional automation to ensure compliance.</b> 

<h2>Skills Demonstrated</h2>

- <b>AWS Security Best Practices: Implementing and enforcing encryption with SSE-S3 and SSE-KMS.</b> 
- <b>AWS KMS Management: Creating and managing KMS keys, policies, and audit logging.</b>
- <b>Automation and Monitoring: Using CloudTrail and Lambda to ensure encryption compliance.(optional) </b>
- <b>Documentation and Compliance: Following security standards and documenting configurations for review. </b>

<h2>Program walk-through:</h2>

<p align="center">
creat your s3 bucket: <br/>
 <img src="image/sc-1.png" height="80%" width="80%" alt="key steps"/>
<br />
 
<br />
Add object to your s3 bucket for Encryption:  <br/>
<img src="image/sc-3.png" height="80%" width="80%" alt="key steps"/>
<br />

<br />
Set Up Default Encryption: Enable SSE-S3 as the default encryption for all objects in the S3 bucket <br/>
<img src="image/sc-4.png" height="80%" width="80%" alt="key steps"/>
<br />

<br />
Override with SSE-KMS: Upload objects with SSE-KMS encryption for enhanced security by specifying the KMS key:  <br/>
<img src="image/sc-5.png" height="80%" width="80%" alt="key steps"/>
<br />
<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>

# high-level-secure-web-architecture
A high level web architecture with cloud security on AWS

## Access the figure here:
https://raw.githubusercontent.com/jklee-github/high-level-secure-web-architecture/main/Figure.png

## Cloud Services selected:
### Identify & Protect
| Services  | Purpose |
| ------------- | ------------- |
|AWS Identity & Access Management (IAM)  | Securely manage access to services and resources|
|Security groups  | Moves security to the instance to provide a stateful, host-level firewall for both web and application servers|
|AWS Shield	|DDoS protection|
|AWS Web Application Firewall (WAF)| Filter malicious web traffic|
|AWS Key Management Service (KMS)	| Key storage and management|
|Amazon Simple Storage Service (Amazon S3) |Secure critical data, static assets, and backups|	

### Detect, Respond & Recover
| Services  | Purpose |
| ------------- | ------------- |
|Amazon GuardDuty|Monitoring the CloudTrail Logs and manage threat detection service, detects potentially compromised instances or reconnaissance by attackers|
|AWS CloudTrail|Track user activity and API usage and provide the logs for Amazon GuardDuty|
|Amazon CloudWatch Event Rule|Triggers an SNS topic and a Lambda function|
|Lambda Function|Isolates the compromised resources (instances, IAM credentials, S3 buckets…) and further properly remediate the resources|
|Amazon SNS|Send admin an e-mail with the finding information|

### Performance and others
| Services  | Purpose |
| ------------- | ------------- |
|Amazon CloudFront|Edge caches high-volume content to decrease the latency to customers|
|Amazon Route 53|Provides DNS services to simplify domain management|
|Elastic Load Balancing|Spread load across multiple Availability Zones|
|Amazon Relational Database Service (Amazon RDS)|Creates a highly available, multi-AZ database architecture|

## Summary
In this Cyber security plan, we first recognize the company's needs and identify the problems to be solved. We utilized the National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF) to fulfill the company's purpose. Lastly, we build a high-level architecture on AWS cloud to align with the company's purpose.

## Reference:
Aligning to the NIST Cybersecurity Framework in the AWS Cloud | Amazon Web Services. (2019). Retrieved 27 February 2022, from https://d1.awsstatic.com/whitepapers/compliance/NIST_Cybersecurity_Framework_CSF.pdf

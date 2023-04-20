# Gportfolio-APP
This project involved hosting a multi-tier web application stack called Gportfolio on AWS cloud production using a lift and shift strategy. It employed various AWS services such as EC2 instances, Elastic Load Balancer, Auto Scaling, S3, Route 53, and IAM user. The flow of execution involved creating key pairs, security groups, launching instances, updating private IP, building the application, and setting up ELB and auto scaling.

AWS SERVICES
Ec2 instances were employed for the creation of VM for Tomcat, RabbitMQ, Memcache, and MySQL services.
Elastic load Balancer (ELb) for the replacement of Nginx Service.
Auto Scaling was used to automatically scale in and out of my instances to control the resources and cost.
S3 was used for storage.
Route 53 was used for Private DNS Services.
IAM User was used in creating an AWS CLI user to SSH into the AWS from my Git bash.


FLOW OF EXECUTION
Login into AWS account
Create key pairs to log into the EC2 Instances
Create Security groups for the load balancer, Tomcat, and backend services.
Launch Instances with User data (Bash Scripts)
Update private IP of backend to name mapping in Route 53.
Build Application from Source Code.
Upload to S3 bucket
Set up ELB to https
Map ELB endpoint to website DNS server on GoDaddy DNS
Build Auto Scaling group for Tomcat Instances


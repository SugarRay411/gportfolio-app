# Gportfolio-APP
The application will host a multi-tier web application stack [Gportfolio] using vagrant. Host and run the project on AWS cloud production. I employed a lift and shift strategy on the project.

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


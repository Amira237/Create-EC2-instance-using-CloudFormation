# Create VPC and EC2 Instance in AWS using CloudFormation

### What is AWS CloudFormation?
##### AWS CloudFormation is a service that helps you model and set up your AWS resources so that you can spend less time managing those resources and more time focusing on your applications that run in AWS. You create a template that describes all the AWS resources that you want (like Amazon EC2 instances or Amazon RDS DB instances), and CloudFormation takes care of provisioning and configuring those resources for you. You don't need to individually create and configure AWS resources and figure out what's dependent on what; CloudFormation handles that. 

### Steps to create VPC and EC2 instance
- **Create VPC (Virtual Private Cloud)** to launch AWS resources into a virtual network
- **Create public subnet** (subnet that's associated with a route table that has a route to an internet gateway) and **private subnet** (a subnet that is associated with a route table that doesn't have a route to an internet gateway)
- **Create Policy Group** that allows SSH and HTTP traffic
- **create gateway**  to access an instance in public subnet
- **create route record**
- **link the route table to the public subnet**
- **Create a new EC2 instance** in the VPC we created with the policy group we added

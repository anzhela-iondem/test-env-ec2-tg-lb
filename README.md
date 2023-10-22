# Test Environment
### AWS Resources
This Terraform code creates two EC2s, Target Group, Load Balancer, and security group with their ingress and egress rules. EC2s have IAM with admin policy, which should be shrunk and adjusted according to the roles and purposes of those EC2s.  

### Bucket
Since the "terraform.tfstate" file is planned to be held in an S3 bucket, an initial S3 bucket named "devops-project-frankfurt" needs to be created.

### Output
The output gives the Load Balancer URL and the private IPs of the EC2s. The IPs can be used in Ansible if we have a server installed in the same VPC network.

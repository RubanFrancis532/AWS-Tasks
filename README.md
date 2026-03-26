Create an EC2 Instance in AWS Console

1. Objective
To create and configure a virtual server using Amazon EC2 and understand basic cloud compute setup.

2. Services Used
Amazon EC2 – Virtual server hosting
AWS Management Console – Web interface to manage AWS resources

3. Architecture Overview
User → AWS Console → EC2 Instance → Internet Access


4. Steps Performed
Step 1: Login to AWS Console
Open AWS Management Console.
Login using root or IAM credentials.
 
Step 2: Navigate to EC2
In the search bar, type EC2.
Select the EC2 service.

Step 3: Launch Instance
Click Launch Instance.
Enter instance details:
Name: My-EC2-Instance
AMI: Amazon Linux
Instance Type: t2.micro

Step 4: Configure Key Pair
Create or select a key pair.
Download the .pem file (used for SSH connection).

Step 5: Configure Network Settings
Select default VPC.
Enable:
SSH (Port 22)
HTTP (Port 80) if needed

Step 6: Configure Storage
Default storage: 8 GB (EBS volume)

Step 7: Launch Instance
Click Launch Instance.
Wait until instance status shows Running.

Step 8: Connect to EC2 Instance
Option 1: EC2 Instance Connect
Select instance
Click Connect → EC2 Instance Connect
Click Connect

Option 2: SSH Connection
ssh -i my-key.pem ec2-user@<public-ip>

5. Verification
Run:
ls
If terminal responds → connection successful ✅

6. Challenges Faced
Incorrect SSH command format
Permission issues with .pem file
Security group not allowing SSH

7. Result
Successfully created and connected to an EC2 instance using AWS Console.

8. Conclusion
This task provided hands-on experience in launching and accessing cloud-based virtual servers using Amazon EC2. It also helped in understanding networking, authentication, and basic instance management.


# Launch-EC2-AWS
Hands-On
Launching an EC2 Instance running Linux

## Steps 
- Login to AWS Console
- Go to EC2 Console
- Click on "Instances"
- Then click "Launch Instances"
- Add a Name and tag (optional)
- Choose a base image (AMI) Amazon Machine Image
- Choose an Architecture ex. AWS and 64 bit
- Choose an Instance Type (t2.micro , c3.large, etc.)
- Create a new Key pair to SSH into the access instance
- Choose a Key pair name ; Key pair type and Private key format (Window OS appropriate)
- Network settings Allow SSH traffic from 0.0.0.0/. (anywhere) and Allow HTTP from the internet
- Configure storage ..... EBS volume size ...
- Advanced details ......
          User data - passing a script to the EC2 instance (run only First time)

  ### Add the following to the User data section and display HTML
   !/bin/bash?
   Use this for your user data (script from top to bottom)
   install httpd (Linux 2 version)
   yum update -y
   yum install -y httpd
   systemctl start httpd
   systemctl enable httpd
   echo "<h1>Hello World from '$'(hostname -f<h1> /var/www/html/index.html")

- Summary 

  >1 Instance 
  >And review the Entity prelaunch
  >Set launch data
  >
  >Next I would like to launch an EC2 instance solely from the AWS CLI or CloudShell

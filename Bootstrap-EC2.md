#Bootstrapping EC2 instances

## EC2 user data is used to automate boot tasks such as:
- Installing updates
- Installing software 
- Downloading common files from the internet
- Anything you can think of really

 > The Boot script > The Boot time >= 0

There are 100s of EC2 instance types


| Instance | vCPU | Mem (GiB)| Storage | Network Performance| EBS Bandwidth (Mbps) |
|---|---|---|---|---|---|
|t2.micro| 1 | 1 | EBS-Only | Low to Moderate | |
|t2.xlarge| 4 | 16 | EBS-Only | Moderate | |
|c5d.4xlarge| 16 | 32 | 1 X 400  NVMe SSD | Up to 10 Gbps | 4750 |
|r5.16xlarge| 64 | 512 | EBS-Only | 20 Gbps | 13,600 |
|m5.8xlarge| 32 | 128 | EBS-Only | 10 Gbps | 6,800 |


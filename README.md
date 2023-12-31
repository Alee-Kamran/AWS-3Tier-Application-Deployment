# AWS 3Tier Application Deployment

# OverView: 
Being an AWS Solution Architect there are 6 pillars of AWS Well-Architect Framework, which plays a vital role in developing a framework. 
These six pillars are as follow: 
i- Operational Excellence 
ii- Security 
iii- Reliability 
iv- Performance Efficiency 
v- Cost Optimization 
vi- Resilience 
In this deployment we will cover Resilient, High-Availability, Security, Fault-Tolerant, and Scalability aspacts. 
To design infrastructure architect, we will use AWS Cloud Platform and its different resources.

# Used Technologies, Services, Tools, and OS: 
GitHub, AWS Cloud, EC2, Security Groups, Route Tables, IGW, NAT, S3, IAM, Ubuntu Local Machine Terminal 
Application Load Balancer, Autoscaling Groups, Nginx, AWS RDS, AMI Templets (Ubuntu Linux Operating System).

# Steps: 
1- Creating VPC 
2: IAM Role (policies) 
3: S3 Bucket (to keep our code) 
4: RDS (Aurora MySQL but for practice purpose we can select MySQL where we can select free tier option) 
5: EC2 Instances 
6: Application Load Balancer 
7: Auto-Scaling Groups (Set-Up Templates)

# Structural Diagram: 
1: we will place Internet Gateway on the edge of our created VPC for public traffic 
2: After Internet Gateway we will create and place our Application Load Balanacer for public traffic to be equally distributed on Public Instances 
3: After ALB our Instances comes (WEB-Layer) 
4: After WEB-Layer Instances we will create and place an other Application Load Balancer for our Next Instance Layer (Application-Layer) 
5: After Internal Application Load Balancer (ALB ) we will create and other set of Instances which will remain Private for Application Code 
6: After this Application-Layer Instances we will create and place our RDS with replication in an other AZ.

# Instructions: 
To keep the cost minimized for study purpose we will design the infrastructure first. 
Our Networking part can be a bit difficult, which you will feel not difficult after doing this Lab. 
While ceating Subnets be very much careful, that you have to come accross Subnets selection several times. 
So Tag or Name your Subnets in a way that you do not get confused while selecting them. 
Just like the Subnets we will be creating different Security Groups too, So please bare in mind that Name or Tag Security Groups wisely 
though you can select those appropriatly when needed.

# Author: Chaudhry Muhammad Ali Kamran 
# Contributors: M. Sajjad, Asad Hanif, Maqbool U Rahman, Sardar Nabil

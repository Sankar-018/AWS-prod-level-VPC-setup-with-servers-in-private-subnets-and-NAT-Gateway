# AWS-prod-level-VPC-setup-with-servers-in-private-subnets-and-NAT-Gateway
This project demonstrates to set up a production-grade AWS Virtual Private Cloud (VPC) with proper network isolation, routing, and secure access architecture. 
Key Implementations

1.Multi-AZ Setup for High Availability

   Deployed EC2 instances in two Availability Zones using an Auto Scaling Group (ASG) to ensure fault tolerance and load distribution
    
2. Private Subnets for EC2 Instances
   
    Application servers are deployed in private subnets, which are not directly exposed to the internet.
   
    Incoming traffic is routed through an Application Load Balancer (ALB) placed in the public subnets.
   
3. Internet Access via NAT Gateway
   
    The EC2 instances in private subnets require outbound internet access (for updates, APIs, etc.).
   
    This is enabled using NAT Gateways, deployed in each Availability Zone for improved redundancy and fault tolerance.    

        
    



        

    

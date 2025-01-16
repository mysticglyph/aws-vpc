#VPC Design and Setup
---------------------
This repository contains the infrastructure setup for production and development networks, designed and built on AWS. The project includes creating distinct Amazon VPCs for both networks, each with specific requirements for subnet design, instance launches, and network connections.

Production Network
-------------------
4-tier Architecture: Designed and implemented a production network with 4 private subnets (app1, app2, dbcache, db) and 1 public subnet (web).
Instance Launches: Instances launched in all subnets, named accordingly.
Internet Access: Allowed dbcache and app1 to send internet requests.
Security: Configured security groups for network management.

Development Network
-------------------
2-tier Architecture: Designed and implemented a development network with 2 subnets (web and db).
Internet Access: Only the web subnet has internet access.
Peering Connection: Set up a peering connection between the production and development networks.
DB Subnet Connectivity: Established a connection between db subnets of both networks.

Technologies Used
----------------
AWS VPC
EC2 Instances
Subnets (Private and Public)
Security Groups
VPC Peering
IAM (Identity and Access Management)

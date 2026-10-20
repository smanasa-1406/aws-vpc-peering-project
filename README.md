# AWS VPC Peering Project

## Project Overview
Implemented a secure AWS networking environment using VPC Peering to establish private communication between two Virtual Private Clouds (VPCs). The project demonstrates AWS networking concepts, secure EC2 access, routing, and connectivity testing.

## Architecture
- **VPC A (10.10.0.0/16):** Contains a public subnet hosting the Bastion Host and a private subnet hosting App-A.
- **VPC B (10.20.0.0/16):** Contains a private subnet hosting App-B.
- **VPC Peering:** Enables private communication between App-A and App-B.
- **Bastion Host:** Provides secure SSH access to private EC2 instances using SSH ProxyJump.

## AWS Technologies Used
- Amazon VPC
- Amazon EC2 (Amazon Linux 2023)
- VPC Peering
- Internet Gateway
- Route Tables and Subnets
- Security Groups
- AWS CloudFormation
- SSH ProxyJump

## Implementation and Testing
- Created two VPCs with non-overlapping CIDR ranges.
- Configured public and private subnets with custom route tables.
- Deployed three EC2 instances: Bastion, App-A, and App-B.
- Established VPC Peering and configured bidirectional routing.
- Verified connectivity before and after peering using ICMP ping tests.
- Tested secure SSH access to private instances through the Bastion Host.
- Performed controlled connectivity failure and recovery testing.
- Documented resource cleanup and EC2 instance termination.

## Project Documentation
📄 [View AWS VPC Peering Project Report](docs/AWS_VPC_Peering_Project_Report.pdf)

## Key Learnings
Gained hands-on experience in AWS VPC networking, private subnet communication, route table configuration, security group management, SSH administration, connectivity troubleshooting, and Infrastructure as Code using AWS CloudFormation.

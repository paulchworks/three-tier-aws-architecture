![image](https://github.com/user-attachments/assets/e9bf95b4-135b-4b61-888b-6d9bcaae8f95)

# Three-tier AWS Architecture

##Both EC2 instances are in private subnets:

TotalAgility instance is in AppSubnet1 (private)

- RPA instance is in AppSubnet2 (private)

## Each application has its own dedicated ALB:

- TotalAgilityALB for the TotalAgility application (listening on port 80)

- RPAALB for the RPA application (listening on port 8080)

## Both ALBs are internet-facing and placed in public subnets:

- They're in PublicSubnet1 and PublicSubnet2

- They have security groups allowing inbound traffic on their respective ports

This architecture follows the best practice of keeping application servers in private subnets for security while exposing services through load balancers in public subnets.

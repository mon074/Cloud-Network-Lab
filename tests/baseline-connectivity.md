# Baseline Connectivity Test

## Objective

Verify that the EC2 instance can communicate with its local
gateway and reach the Internet.

## EC2 Network Information

- VPC CIDR: 10.0.0.0/16
- Subnet CIDR: 10.0.1.0/24
- Availability Zone: ap-south-1b
- EC2 Private IP: 10.0.1.6
- Network Interface: ens5
- Default Gateway: 10.0.1.1

## Linux Routing

The EC2 routing table contains:

- 10.0.1.0/24 → directly connected through ens5
- Default route → 10.0.1.1

## Connectivity Tests

### Local Gateway
Command: ping -c 4 10.0.1.1
Result: PASS

### Internet Connectivity
Command: ping -c 4 8.8.8.8
Result: PASS

#### DNS Resolution
Command: nslookup google.com
Result: PASS

### HTTPS Connectivity
Command: curl -I https://google.com
Result: PASS
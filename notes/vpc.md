# VPC Configuration

## Overview

The first step of the Cloud Network Lab was to create an isolated Amazon VPC for networking and troubleshooting practice.

## Configuration

VPC Name-> Cloud-Network-Lab 
IPv4 CIDR-> 10.0.0.0/16 
Purpose-> Isolated AWS network for troubleshooting lab 

## Why VPC?

An Amazon VPC provides an isolated virtual network in AWS where resources such as EC2 instances can be deployed and controlled using subnets, route tables, and other networking components.

## CIDR Block

The VPC uses: 10.0.0.0/16

This provides a private IPv4 address range that can be divided into smaller subnet ranges.

Key Learning
- A VPC is the fundamental networking boundary in AWS.
- CIDR defines the IP address range available inside the VPC.
- Subnets are created within the VPC CIDR range.
- Route tables control how network traffic is directed.

please refer to screenshots to see all the configurations!
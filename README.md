# Active-Directory-Home-Lab
📌 Project Overview

This project simulates a small business domain environment using a virtualized Windows Server infrastructure. I built and configured a Domain Controller, joined a client machine to the domain, created user accounts and security groups, and implemented Group Policy settings to replicate common IT Support and system administration tasks.

The purpose of this lab was to gain hands-on experience with Active Directory administration, user lifecycle management, access control, and troubleshooting domain connectivity issues.

🛠 Technologies Used

VirtualBox

Windows Server 2022 (Evaluation)

Windows 10 (Client VM)

Active Directory Domain Services (AD DS)

Group Policy Management

DNS & DHCP

Command Prompt / PowerShell

🏗 Lab Architecture

1 Domain Controller (Windows Server 2022)

1 Windows 10 Client Machine

Internal Virtual Network

Domain: corp.local

🎯 Objectives

Install and configure Windows Server

Promote server to Domain Controller

Configure DNS

Create Organizational Units (OUs)

Create users and security groups

Configure password policies

Join client machine to domain

Configure shared folders and NTFS permissions

Simulate common help desk tasks

🔧 Key Tasks Performed
1️⃣ Domain Controller Setup

Installed Windows Server 2022

Assigned static IP address

Installed Active Directory Domain Services role

Promoted server to Domain Controller

Created new forest: corp.local

2️⃣ User & Group Management

Created 10 test user accounts

Organized users into OUs (HR, Sales, IT)

Created security groups for role-based access

Assigned users to appropriate groups

3️⃣ Group Policy Configuration

Configured password complexity requirements

Set account lockout threshold

Restricted control panel access for standard users

Forced password change at next login

4️⃣ Shared Folder Permissions

Created shared network drive

Configured NTFS permissions

Applied least-privilege access model

Verified access from client machine

5️⃣ Client Domain Join

Joined Windows 10 machine to domain

Verified domain login functionality

Tested user access restrictions

🧪 Troubleshooting Scenarios
❗ Issue: Client Could Not Join Domain

Diagnosis: DNS server not pointing to Domain Controller
Resolution: Updated client DNS settings to DC IP address

❗ Issue: User Locked Out

Diagnosis: Exceeded password attempts threshold
Resolution: Unlocked account via AD Users & Computers

❗ Issue: Shared Folder Access Denied

Diagnosis: User not added to proper security group
Resolution: Updated group membership and refreshed policy

🔐 Security Concepts Practiced

Role-Based Access Control (RBAC)

Least Privilege Principle

Password Policy Enforcement

Account Lockout Policies

Secure DNS Configuration

📚 Key Takeaways

DNS is critical in domain environments

Group Policy is powerful for enforcing security standards

Proper OU structure simplifies user management

Documentation is essential for troubleshooting efficiency

🚀 Next Steps

Expand lab with additional client machines

Implement Group Policy software deployment

Practice PowerShell user creation automation

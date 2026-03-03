# Active-Directory-Home-Lab
# Overview
This project demonstrates setting up a Windows Server Active Directory lab in a virtual environment.

The lab covers:

- Windows Server Installation
- Active Directory Domain Services setup
- Domain Controller creation
- Domain Admin login
- Organizational Units (OUs) creation
- User creation
- Group membership configuration
- Password policy configuration
- Audit policy configuration
- Security event log monitoring
- Simulated failed and successful logins

This lab simulates a realistic enterprise Active Directory environment and demonstrates both configuration and troubleshooting skills.

# Lab Architecture

Domain Controller:
- Windows Server 2022
- Static IP: 192.168.50.10
- Domain: corp.local

Client Machine:
- Windows 11 Pro
- Joined to corp.local

**Virtualization** VirtualBox

# Step-by-Step Screenshots

1. Server Installed
![Server Installed](01-server-install.png)
Installed Windows Server 2022 as the foundation for the lab.

2. Active Directory Role Installed
![AD DS Installed](02-add-ad-role.png)
Added Active Directory Domain Services (AD DS) role to the server.

3. Domain Created
![Domain Created](03-domain-created.png)
Promoted the server to a Domain Controller and created the 'corp.local' domain.

4. Domain Admin Login
![Domain Admin Login](04-domain-admin-login.png)
Logged in as the domain administrator to verify the domain creation was successful.

5. Organizational Units Created
![OUs Created](05-ous-created.png)
Created organizational units (OUs) to organize users and computers for easier management.

6. Users Created
![Users Created](06-users-created.png)
Created test users within the OUs to simulate real-world accounts.

7. Group Membership Configured
![Group Membership](07-group-membership.png)
Assigned users to appropriate groups, demonstrating access control management.

8. Password Policy Set
![Password Policy](08-password-policy.png)
Configured password policies to enforce security best practices.

9. Audit Enabled
![Audit Enabled](09-audit-enabled.png)
Enabled auditing policies to monitor logon events, account management, and policy enforcement.

10. Failed Login Attempt
![Failed Login](10-failed-login.png)
Simulated a failed login to generate audit events for security monitoring.

11. Successful Login
![Successful Login](11-successful-login.png)
Verified successful login for a test user and captured the corresponding security event.

# Security Event IDs Observed
- 4624 - Successful Login
- 4625 - Failed Login
- 4723 - Password Change Attempt
- 4724 - Password Reset

These events demonstrate that auditing is functional and properly logging key domain activities.
# Skills Demonstrated
- Windows Server Administration
- Active Directory Administration
- Organizational Unit (OU) Creation
- User and Group Management
- Password Policy Configuration
- Audit Policy Setup
- Security Event Monitoring
- **Domain Environment Troubleshooting** - verified domain creation, user access, group policies, and audit logs to identify and resolve issues.

## How to Use This Repo
This repository contains step-by-step screenshots and descriptions of an Active Directory lab environment. Each screenshot corresponds to a specific lab task.
To view the lab flow, follow the screenshots in numerical order from '01-server-install.png' through '11-successful-login.png'.


# IAM Active Directory Lab
## Overview
This project simulates an enterprise identity and access management (IAM) environment using Active Directory.

Technologies Used
- Windows Server 2022
- Active Directory Domain Services
- PowerShell

Key Tasks Performed
- Installed and configured Active Directory Domain Controller
- Created and managed user accounts
- Implemented role-based access control (RBAC) using security groups
- Automated user provisioning using PowerShell

Sample PowerShell Commands
powershell Import-Module ActiveDirectory  New-ADUser -Name "Jane Smith" -GivenName "Jane" -Surname "Smith" -SamAccountName "jsmith" -UserPrincipalName "jsmith@corp.local" -AccountPassword (ConvertTo-SecureString "Password123!" -AsPlainText -Force) -Enabled $true  Add-ADGroupMember -Identity "HR_Access" -Members "jsmith" 

What I Learned
- Identity lifecycle management (provisioning/deprovisioning)
- Role-based access control (RBAC)
- IAM automation using PowerShell## Project Scenario

This lab simulates a real world IAM scenario where new employees are onboarded into an organization. User accounts are created, assigned to role based security groups, and managed using both GUI and PowerShell automation.
Skills Demonstrated
- User provisioning and deprovisioning
- Role-Based Access Control (RBAC)
- Active Directory administration
- PowerShell automation for identity management

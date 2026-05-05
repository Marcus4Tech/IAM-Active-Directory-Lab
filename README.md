IAM Active Directory Lab

Overview
This project simulates an enterprise Identity and Access Management (IAM) environment using Active Directory. The lab focuses on user provisioning, access control, and automation of identity-related tasks.

Environment
- Windows Server 2022
- Active Directory Domain Services (AD DS)
- PowerShell

Project Scenario
This lab simulates a real-world IAM scenario where new employees are onboarded into an organization. User accounts are created, assigned to role-based security groups, and managed using both GUI and PowerShell automation.

Key Tasks Performed
- Installed and configured a Windows Server 2022 Domain Controller
- Created and managed user accounts in Active Directory
- Implemented role-based access control (RBAC) using security groups
- Automated user provisioning and access assignment using PowerShell

PowerShell Automation Example
powershell Import-Module ActiveDirectory  New-ADUser -Name "Jane Smith" -GivenName "Jane" -Surname "Smith" ` -SamAccountName "jsmith" -UserPrincipalName "jsmith@corp.local" ` -AccountPassword (ConvertTo-SecureString "Password123!" -AsPlainText -Force) -Enabled $true  Add-ADGroupMember -Identity "HR_Access" -Members "jsmith" 

Skills Demonstrated
- Identity Lifecycle Management (Provisioning/Deprovisioning)
- Active Directory Administration
- Role-Based Access Control (RBAC)
- PowerShell Automation

Future Improvements
- Bulk user provisioning using CSV files
- Integration with Microsoft Entra ID
- Access review and audit simulation
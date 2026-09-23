# Windows Server & Active Directory Home Lab

## Overview

This project is a hands-on IT administration lab built using Oracle VirtualBox and Windows Server.

The goal of this lab is to simulate a small business IT environment and develop practical skills in:

- Windows Server administration
- Active Directory Domain Services (AD DS)
- DNS
- User and group management
- Organizational Units (OUs)
- Security groups
- Account administration
- Password resets
- User troubleshooting
- Help desk support
- Group Policy
- Windows client/domain administration

This lab is designed to simulate the type of environment an entry-level IT Support Specialist, Help Desk Technician, Desktop Support Technician, or Junior System Administrator may encounter.

---

## Lab Environment

| Component | Configuration |
|---|---|
| Hypervisor | Oracle VirtualBox |
| Server OS | Windows Server |
| Domain | `DIAZCRUZ.LOCAL` |
| Domain Controller | `Diaz-Cruz2026` |
| Directory Service | Active Directory Domain Services |
| DNS | Windows Server DNS |
| Departments | HR, IT, Warehouse, Sales |
| User Accounts | 25 fictional employees |

---

## Active Directory Structure

The domain contains the following Organizational Units:


DIAZCRUZ.LOCAL
|---|
├── HR
├── IT
├── Warehouse
├── Sales
├── Computers
├── Service Accounts
├── Groups




## Security Groups

The following security groups were created:

### Company-Wide

- All-Employees

### HR

- HR-Users
- HR-Managers

### IT

- IT-Users
- IT-Admins
- IT-Managers

### Warehouse

- Warehouse-Users
- Warehouse-Managers

### Sales

- Sales-Users
- Sales-Managers

These groups are used to simulate role-based access management within the organization.



## User Management

The lab currently contains 25 fictional employee accounts distributed across four departments:

- HR
- IT
- Warehouse
- Sales

User accounts were created with standardized usernames and assigned to their appropriate departmental OUs and security groups.



## Active Directory Administration Tasks

Hands-on tasks completed or planned in this lab include:

- Creating user accounts
- Creating Organizational Units
- Creating security groups
- Adding users to security groups
- Enabling disabled accounts
- Resetting user passwords
- Requiring password changes at next logon
- Troubleshooting authentication issues
- Managing departmental organization
- DNS troubleshooting
- Domain administration



## DNS Troubleshooting

During initial server configuration, DNS resolution was tested using:

 ping 8.8.8.8<br>
 ping google.com<br>
 nslookup google.com<br>
ipconfig /flushdns<br>

  


Testing connectivity by IP address and hostname helped distinguish between general network connectivity and DNS resolution problems.



## Help Desk Integration

This Active Directory environment is being integrated with a separate Jira Service Management help desk simulation.

The purpose is to practice the complete IT support workflow:

<center>
User reports problem<br>
        ↓<br>
Help Desk receives ticket<br>
        ↓<br>
Troubleshoot issue<br>
        ↓<br>
Investigate Active Directory<br>
        ↓<br>
Make appropriate change<br>
        ↓<br>
Verify resolution<br>
        ↓<br>
Document work<br>
        ↓<br>
Resolve ticket
</center>




## Example Support Scenario

### Account Access Issue

A simulated HR employee was unable to log into Windows and received an error indicating that the account may be locked out.

Investigation in Active Directory showed that the account was actually disabled.

The account was re-enabled, but the user continued receiving a username/password authentication error.

The user's password was subsequently reset and the user was required to create a new password at next logon.

The user successfully logged into Windows and confirmed that access had been restored.

### Skills Demonstrated

- Active Directory user investigation
- Account status verification
- Account re-enablement
- Password reset
- Authentication troubleshooting
- User communication
- Ticket documentation
- Resolution verification



## Planned Lab Exercises

Future exercises will include:

- Creating a Windows 11 client VM
- Joining a Windows 11 client to the domain
- Creating Group Policy Objects (GPOs)
- Applying departmental policies
- Testing user permissions
- File and folder access control
- Account lockout troubleshooting
- Password policy configuration
- Software deployment concepts
- Printer troubleshooting
- Network troubleshooting
- Help desk ticket simulations
- Windows client troubleshooting



## Tools Used

- Windows Server
- Oracle VirtualBox
- Active Directory Users and Computers
- DNS Manager
- Server Manager
- Command Prompt
- PowerShell
- Jira Service Management



## Project Goals

The primary goal of this project is to develop practical experience with common IT support and system administration tasks in a controlled lab environment.

This project is continuously being expanded with new troubleshooting scenarios, documentation, and simulated business requirements.



## Disclaimer

This is a personal educational lab using fictional users and simulated company data.

No real customer, employee, password, or confidential company information is stored in this repository.

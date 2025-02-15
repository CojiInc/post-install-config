# osTicket - Post-Install Configuration

<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

## Overview
This guide outlines the post-installation configuration steps for osTicket, ensuring the help desk system is properly set up for use.

### Video Demonstration
- [YouTube: How To Configure osTicket, Post-Installation](https://www.youtube.com)

## Environment and Technologies Used
- **Microsoft Azure** (Virtual Machines/Compute)
- **Remote Desktop**
- **Internet Information Services (IIS)**
- **Windows 10 (21H2)**

## Post-Installation Configuration Steps

### 1. Accessing osTicket
- **Admin/Analyst Login Page**: [http://localhost/osTicket/scp/login.php](http://localhost/osTicket/scp/login.php)
- **End Users osTicket URL**: [http://localhost/osTicket](http://localhost/osTicket)
- Acknowledge the difference between the **Agent Panel** (ticket handling) and **Admin Panel** (system management).

### 2. Configure User Roles and Permissions
- **Roles (Permissions Groups)**  
  - Navigate to: `Admin Panel → Agents → Roles`
  - Create `Supreme Admin` role for full control.

- **Departments (Ticket Visibility & Management)**  
  - Navigate to: `Admin Panel → Agents → Departments`
  - Create `SysAdmins` department.

- **Teams (Cross-Department Collaboration)**  
  - Navigate to: `Admin Panel → Agents → Teams`
  - Create `Online Banking` team with agents from different departments.

### 3. Configuring Ticket Handling Settings
- **Allow Anyone to Create Tickets**  
  - Navigate to: `Admin Panel → Settings → User Settings`
  - **Uncheck** "Unregistered users can create tickets" to restrict access.
  - Enable "Registration Required" to require users to log in before creating tickets.

- **Add Agents (Help Desk Staff)**  
  - Navigate to: `Admin Panel → Agents → Add New`
  - Create:
    - **Jane** (Department: SysAdmins)
    - **John** (Department: Support)

- **Add Users (End-Users/Customers)**  
  - Navigate to: `Agent Panel → Users → Add New`
  - Create:
    - **Karen**
    - **Ken**

### 4. Service Level Agreements (SLAs)
- Navigate to: `Admin Panel → Manage → SLA`
- Set up SLAs for response times:
  - **Sev-A** (Grace Period: 1 hour, Schedule: 24/7)
  - **Sev-B** (Grace Period: 4 hours, Schedule: 24/7)
  - **Sev-C** (Grace Period: 8 hours, Business Hours)

### 5. Configure Help Topics  
- Navigate to: `Admin Panel → Manage → Help Topics`
- Add help topics for users to categorize their issues:
  - **Business Critical Outage**
  - **Personal Computer Issues**
  - **Equipment Request**
  - **Password Reset**
  - **Other**

---

## Final Steps & Best Practices
- **Test Ticket Creation & Assignment**
- **Explore Email Notifications for Ticket Updates**
- **Understand Ticket Intake Methods** (Phone, Chat, Web, Email)
- **Practice Working Tickets to Completion**
- **Repeat the Lab to Build Confidence**

## 🎉 Congratulations!
Your osTicket system is now fully configured and ready for use! 🚀


# osTicket - Post-Install Configuration

<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

## osTicket - Post-Install Configuration
This section covers the post-installation configuration steps to set up osTicket for help desk operations.

### Video Demonstration
- [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

## Post-Install Configuration Objectives
- Change SysAdmins Department to a Top-Level Department
- Delete the Maintenance Department (not archive)
- Configure ticket properties for different requests
- Work tickets to completion as different agents

## Configuration Steps
### 1. Logging In
- **Admin/Analyst Login Page**: [http://localhost/osTicket/scp/login.php](http://localhost/osTicket/scp/login.php)
- **End Users osTicket URL**: [http://localhost/osTicket](http://localhost/osTicket)

### 2. Create and Manage Tickets
#### Ticket 1: Online Banking System Down
- Create a ticket as an end-user: `Entire mobile/online banking system is down`
- As Agent (John), observe ticket properties and set:
  - **Priority:** Sev-A (1 hour, 24/7)
  - **Department:** Online Banking Department
- Check ticket access after assignment
- Work ticket to completion as Jane

#### Ticket 2: Adobe Upgrade Issue
- Create a ticket: `Accounting department needs Adobe upgrade, broken`
- As Agent (John), set:
  - **Priority:** Sev-B (4 hours, 24/7)
  - **Department:** Support
- Work ticket to completion as John

#### Ticket 3: CFO’s Laptop Won’t Turn On
- Create a ticket: `CFO’s laptop will no longer turn on`
- As Agent (John), set:
  - **Priority:** Sev-B (4 hours, 24/7)
  - **Department:** Support
- Work ticket to completion as John

### 3. Ticket Escalation and Permissions
- Set Properties to all tickets; observe SysAdmins ticket becomes inaccessible
- Assign yourself view-access to SysAdmins department in **Admin Panel**
- Switch back to Agent Panel and observe changes

### 4. Ticketing System Best Practices
- Explain how email notifications work in most ticketing systems
- Discuss ticket intake methods (phone, chat, email, web form, etc.)
- Stress importance of logging all issues for tracking and metrics

## Conclusion
- Encourage further exploration of osTicket’s features
- Recommend repeating the lab to build confidence and intuition
- Reinforce the importance of technical proficiency through repeated practice

## Congratulations! 🎉
Your osTicket helpdesk is now successfully configured!


# Modern Microsoft 365 Endpoint Management Lab

## Project Overview

This project demonstrates how modern organisations manage identities, devices, security and messaging services using Microsoft 365 cloud technologies.

The lab simulates a corporate environment where Windows devices are enrolled into Microsoft Intune, secured using device compliance policies and Conditional Access, provisioned using Windows Autopilot, and connected to Microsoft 365 services such as Exchange Online.

User identities are managed through Microsoft Entra ID, devices are enrolled and secured using Microsoft Intune, and email services are administered through Exchange Online.

Key tasks performed in this project included identity administration, device enrollment, security policy configuration, mailbox administration, troubleshooting email delivery using message trace, and configuring Windows Autopilot for automated device provisioning.

The objective of this project was to gain practical experience with the Microsoft 365 endpoint management ecosystem and understand how these services work together to manage users, secure endpoints and automate device deployment in modern enterprise environments.

---

## Table of Contents

- [Lab Environment](#lab-environment)
- [Architecture Overview](#architecture-overview)
- [Identity Management (Entra ID)](#identity-management-entra-id)
- [Device Enrollment (Intune)](#device-enrollment-intune)
- [Device Security (Compliance + Conditional Access)](#device-security-compliance--conditional-access)
- [Exchange Online Administration](#exchange-online-administration)
- [Windows Autopilot Deployment](#windows-autopilot-deployment)
- [Helpdesk Scenarios Simulated](#helpdesk-scenarios-simulated)
- [Key Skills Demonstrated](#key-skills-demonstrated)

---

## Lab Environment

The lab environment was built using the following components:

- Microsoft 365 Business Premium tenant  
- Microsoft Entra ID  
- Microsoft Intune  
- Exchange Online  
- Windows Autopilot  
- Windows 11 Virtual Machine (VMware Workstation)

This environment simulates how organisations manage users, devices and security within a modern cloud-managed Microsoft 365 environment.

---

## Architecture Overview

The lab demonstrates how identity, device management, security policies and messaging services integrate within the Microsoft 365 ecosystem.

User Identity → Microsoft Entra ID → Intune Device Management → Compliance Policies → Conditional Access → Exchange Online

Autopilot is used to automate device provisioning during the initial setup process.

---

## Identity Management (Entra ID)

The project began with configuring identity management using Microsoft Entra ID.

Tasks performed:

- Created user accounts within Entra ID  
- Assigned Microsoft 365 licenses  
- Reset user passwords  
- Disabled and re-enabled user accounts  
- Reviewed sign-in logs to monitor authentication activity  

This step demonstrates how organisations manage identities and control access within Microsoft 365.

### User Created
![User Created](./screenshots/user-created.png)

### License Assigned
![License Assigned](./screenshots/license-assigned.png)

### Password Reset
![Password Reset](./screenshots/password-reset.png)

### Account Disabled
![Account Disabled](./screenshots/account-disabled.png)

### Sign-in Logs
![Sign-in Logs](./screenshots/signin-logs.png)

---

## Device Enrollment (Intune)

A Windows 11 virtual machine was enrolled into Microsoft Intune to simulate a corporate managed device.

### Tasks Performed:

- Enrolled a Windows 11 virtual machine into Microsoft Intune via Microsoft Entra ID
- Verified successful device registration in Microsoft Entra ID  
- Confirmed device visibility within Microsoft Intune device inventory  
- Applied and reviewed a compliance policy to the enrolled device  
- Validated device compliance status as “Compliant” within Intune  
- Monitored device check-in status to ensure active communication with Intune  

Device enrollment allows administrators to manage devices centrally using security policies and configuration profiles.
### Device Enrolled (Work Account Connected)
![Device Enrolled](./screenshots/device-enrolled.png)

### Device Registered in Entra ID
![Entra Device](./screenshots/entra-device-list.png)

### Device Listed in Intune
![Intune Device](./screenshots/intune-device-list.png)

### Compliance Policy Applied
![Compliance Policy](./screenshots/compliance-policy.png)

### Device Compliance Status
![Device Compliance](./screenshots/device-compliance.png)

---

## Device Security (Compliance + Conditional Access)

Device security policies were implemented using Microsoft Intune compliance policies and Microsoft Entra Conditional Access.

### Tasks Performed:

- Created a Windows compliance policy in Microsoft Intune to enforce device security requirements  
- Evaluated device compliance against configured policy settings  
- Verified that the enrolled device met compliance requirements within Intune  
- Created a Conditional Access policy in Microsoft Entra ID targeting Microsoft 365 applications  
- Configured grant controls to require devices to be marked as compliant before access is granted  
- Tested and validated that access to resources is restricted based on device compliance status

### Compliance Policy
![Compliance Policy](./screenshots/compliance-policy.png)

### Device Compliance Status
![Device Compliance](./screenshots/device-compliance.png)

### Conditional Access Policy Overview
![Conditional Access Policy](./screenshots/conditional-access-policy.png)

### Conditional Access Assignments
![Conditional Access Assignments](./screenshots/conditional-access-assignments.png)

### Grant Controls (Require Compliant Device)
![Grant Controls](./screenshots/grant-controls.png)


## Exchange Online Administration

Exchange Online was configured to simulate common helpdesk and administration tasks.

Tasks performed:

- Created a shared mailbox  
- Assigned mailbox delegation (Full Access and Send As permissions)  
- Converted a user mailbox to a shared mailbox  
- Removed a license while preserving mailbox data  
- Used Message Trace to troubleshoot email delivery  

These tasks demonstrate common email administration and troubleshooting processes used in enterprise environments.

### Shared Mailbox Created
![Shared Mailbox](./screenshots/shared-mailbox.png)

### Mailbox Permissions (Send As)
![Send As Permission](./screenshots/send-as-permission.png)

### Mailbox Permissions (Full Access)
![Full Access Permission](./screenshots/full-access-permission.png)

### Mailbox Converted to Shared
![Mailbox Conversion](./screenshots/mailbox-after-conversion.png)

### License Removed (Mailbox Preserved)
![License Removed](./screenshots/license-removed.png)

### Shared Mailbox Email Test
![Shared Mailbox Send](./screenshots/shared-mailbox-send.png)

### Message Trace (Email Delivery Verified)
![Message Trace](./screenshots/message-trace.png)

---

## Windows Autopilot Deployment

Windows Autopilot was explored to understand how devices can be provisioned and configured automatically in a modern enterprise environment.

Although the device in this lab was enrolled directly into Microsoft Intune, an Autopilot deployment profile was created and configured to demonstrate knowledge of automated provisioning workflows.

### Tasks Performed:

- Created a Windows Autopilot deployment profile  
- Configured Out-of-Box Experience (OOBE) settings  
- Assigned the deployment profile to devices  
- Reviewed deployment configuration options for automated device provisioning  

### Autopilot Deployment Profile
![Autopilot Profile](./screenshots/autopilot-profile.png)

### OOBE Configuration
![Autopilot OOBE](./screenshots/autopilot-oobe.png)

---


## Key Skills Demonstrated

- Microsoft Entra ID administration  
- Microsoft Intune device management  
- Conditional Access policy configuration  
- Windows device compliance management  
- Exchange Online mailbox administration  
- Windows Autopilot deployment configuration  
- Microsoft 365 troubleshooting



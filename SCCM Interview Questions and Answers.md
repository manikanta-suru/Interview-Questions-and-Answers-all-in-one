# SCCM Interview Questions and Answers

This repository contains a comprehensive list of **SCCM (System Center Configuration Manager)** interview questions and answers for both **freshers** and **experienced professionals**.

---

## Table of Contents
1. [Freshers Questions](#freshers-questions)
2. [Experienced Questions](#experienced-questions)
3. [SCCM Administrator Questions](#sccm-administrator-questions)
4. [SCCM Patch Management Questions](#sccm-patch-management-questions)

---

## Freshers Questions

### 1. What is SCCM?
- **Answer:** System Center Configuration Manager (SCCM) is a software management tool developed by Microsoft. It allows users to manage computers running Windows, Linux, and macOS. SCCM is also known as ConfigMgr.

### 2. What are the essential features of SCCM?
- **Answer:** The essential features of SCCM include:
  - Desired Configuration Management
  - Asset tracking
  - Deployment of operating systems
  - Reporting
  - Software deployment
  - Remote control
  - Patch management.

### 3. List out the various types of sites available in SCCM.
- **Answer:** The types of sites in SCCM are:
  - Primary site
  - Central Administration site
  - Secondary site.

### 4. What is the Central Administration Site (CAS)?
- **Answer:** The Central Administration Site (CAS) is the top-level site in SCCM. It supports only primary sites as child sites and is used to manage all clients in the hierarchy.

### 5. What is the difference between the Primary site and a Secondary site?
- **Answer:**

| **Primary Site**                          | **Secondary Site**                          |
|-------------------------------------------|---------------------------------------------|
| Can access the Microsoft SQL Database.    | Cannot access the Microsoft SQL Database.   |
| Can be administered through the SCCM console. | Can only be administered through the Primary Site. |
| Can have child sites.                     | Cannot have child sites.                    |
| Clients can be assigned directly.         | Clients cannot be assigned directly.        |

### 6. Define Child site in SCCM.
- **Answer:** A child site is a site that gets all its data from a higher-level site (e.g., a primary site or CAS).

### 7. Why do we use BITS in SCCM?
- **Answer:** Background Intelligent Transfer Service (BITS) is used to transfer data between the SCCM server and clients. It is also used to download the SCCM client to machines during client push installation.

### 8. Define SUP.
- **Answer:** Software Update Point (SUP) is a site system role used to create software update backgrounds. It integrates with WSUS to manage software updates.

### 9. Why do we use WSUS, and what is it?
- **Answer:** Windows Server Update Services (WSUS) is used to deploy updates to systems running Windows OS. It works with SCCM to manage software updates.

### 10. Define SMS providers in SCCM.
- **Answer:** SMS providers are used to access the SCCM database. They can be installed on the site database server, site server, or another server during SCCM setup.

### 11. List various client deployment methods.
- **Answer:** The client deployment methods are:
  - Client push installation
  - Group Policy installation
  - Manual installation
  - Software update point-based installation
  - Upgrade installation
  - Logon script installation.

### 12. List the ports used in SCCM.
- **Answer:** The ports used in SCCM are:
  - TCP 2701
  - Default HTTPS port 443
  - Client to site system HTTP port 80
  - SMB 445.

### 13. What are the types of the sender in SCCM?
- **Answer:** The types of senders in SCCM are:
  - Standard Sender
  - Courier Sender.

### 14. What are the different application detection methods defined in SCCM?
- **Answer:** The application detection methods are:
  - Registry
  - Custom detection
  - Windows installers
  - File system.

### 15. Define the fallback status point in SCCM.
- **Answer:** The fallback status point provides Configuration Manager clients with alternative servers when the client site assignment or installation fails.

### 16. What is Deployment Share SCCM?
- **Answer:** The deployment share in SCCM is a repository for applications, OS images, device drivers, and language packs. It can be deployed to target machines.

### 17. Why do we use Server Locator Point in SCCM?
- **Answer:** Server Locator Points help clients find their assigned site and management points when they cannot retrieve this information through Active Directory Domain Services.

### 18. Mention some of the important site system roles in SCCM.
- **Answer:** The important site system roles in SCCM are:
  - Distribution point
  - Fallback status point
  - Management point
  - PXE service point
  - Reporting point
  - Server locator point
  - Software update point
  - State migration point.

### 19. List the services required for the client computer to communicate with the server.
- **Answer:** The services required are:
  - Computer browser
  - SMS agent host
  - WMI
  - Windows installer
  - Background Intelligent Transfer Server (BITS).

### 20. What is the SCCM console?
- **Answer:** The SCCM console is a tool used to perform tasks such as device management, network management, and application deployment.

---

## Experienced Questions

### 23. How to backup SCCM Server?
- **Answer:** To back up the SCCM server, expand the **Site Maintenance** and **Site Setting** nodes in the SCCM console, and click on specific tasks you want to back up.

### 24. How to distribute the package?
- **Answer:** To distribute a package:
  1. Write an install program to create the package in SCCM.
  2. Assign distribution points to the package.
  3. Create a collection to receive the package.
  4. Create an advertisement for distribution.

### 25. What are the new features in the release of SCCM 1806?
- **Answer:** The new features in SCCM 1806 include:
  - Site server high availability
  - CMPivot
  - Enable distribution points to use network congestion control
  - Enhanced HTTP site system
  - Download content from a CMG
  - Improved WSUS maintenance
  - Phased deployment of applications.

### 26. How to connect the SCCM site server?
- **Answer:** To connect to the SCCM site server using PowerShell:
  1. Open PowerShell as Administrator.
  2. Run the command to connect to the site server.
  3. Enter the site code to enable the connection.

### 27. Define ITMU.
- **Answer:** ITMU (Inventory Tool for Microsoft Updates) is used for SMS 2003 to manage software updates.

### 28. What is the latest version of SCCM?
- **Answer:** The latest version of SCCM is **Endpoint Configuration Manager 2002**, released in April 2020.

### 29. What are the features of the latest version of SCCM?
- **Answer:** The features include:
  - Application management
  - Real-time management
  - Microsoft Endpoint Manager tenant attach
  - Desktop Analytics
  - Site infrastructure
  - Client management
  - Content management.

### 30. What are All Unknown Computers collections?
- **Answer:** The All Unknown Computers collection includes devices not managed by SCCM. It is used to deploy operating systems to unmanaged systems.

---

## SCCM Administrator Questions

### 51. Why do we use the cloud management dashboard?
- **Answer:** The cloud management dashboard provides a centralized view of cloud management gateway usage and helps troubleshoot issues in real-time.

### 52. Define inventory in SCCM.
- **Answer:** Inventory in SCCM provides system information such as the operating system, processor type, and applications. It includes:
  - Hardware inventory
  - Software inventory.

---

## SCCM Patch Management Questions

### 80. What is IMTU patch management?
- **Answer:** IMTU patch management involves:
  - Scanning using Windows Update Agent (WUA).
  - Using WSUS as a scan inventory (SUP).
  - Downloading only required updates.
  - Installing non-security updates after defining security updates in WSUS.

As of May 2025, the latest SCCM (System Center Configuration Manager) client agent version is 5.00.9158.1000, which corresponds to Configuration Manager Current Branch version 2503.

📌 SCCM 2503 Client Agent Version Details
Client Version: 5.00.9158.1000

Release Date: March 31, 2025

Support End Date: September 30, 2026

Update Type: In-console update for sites running version 2309 or later
Prajwal Desai
Reddit
+8
Reddit
+8
Microsoft Learn
+8

This update focuses on security and quality improvements, addressing over 230 reported bugs. 
Prajwal Desai
+1
Reddit
+1

🔄 How to Verify and Upgrade the SCCM Client Version
Check Current Client Version:

On a client machine, open the Control Panel.

Navigate to Configuration Manager > General tab.

The client version is displayed here.

Enable Automatic Client Upgrade:

Open the SCCM Console.

Go to Administration > Site Configuration > Sites.

Select your site and click on Hierarchy Settings in the ribbon.

Under the Client Upgrade tab, check the box for Upgrade all clients in the hierarchy using production client.

Specify the number of days for the upgrade to occur.
System Center Dudes
+1
Prajwal.org
+1
Lansweeper

Manual Client Upgrade:

Download the latest client installation package from the SCCM site server.

Run the installer on the target client machines.

🛠️ Troubleshooting Tips
Client Not Updating:

Ensure the client machine has network connectivity to the SCCM server.

Check for any firewall rules blocking communication.

Review the ccmsetup.log file on the client for installation errors.

Version Mismatch:

Use the following WQL query to identify clients not on the latest version:
Prajwal.org

sql
Copy
Edit
SELECT SMS_R_System.Name, SMS_R_System.ClientVersion
FROM SMS_R_System
WHERE SMS_R_System.ClientVersion != '5.00.9158.1000'


---

## Conclusion
This repository is a comprehensive resource for SCCM interview preparation. Feel free to contribute or suggest improvements!

# 🔐 Microsoft Entra ID Overview

Microsoft **Entra ID** (formerly **Azure Active Directory**) is a cloud-based Identity and Access Management (IAM) service from Microsoft. It helps organizations securely manage **users**, **devices**, and **access** to apps and data — both on-premises and in the cloud.

---

## 🚀 Key Features

| 🔧 Feature                | 📝 Description                                                                 |
|--------------------------|--------------------------------------------------------------------------------|
| 🔐 **Single Sign-On (SSO)**   | Access all your apps with one login.                                           |
| 📱 **Multi-Factor Authentication (MFA)** | Add an extra layer of security during sign-ins.                          |
| 🌍 **Conditional Access**   | Apply policies based on user, device, location, and risk.                    |
| 🔄 **Self-Service Password Reset** | Reduce IT overhead by letting users reset their own passwords.           |
| 🧩 **App Integration**     | Works with Microsoft 365, Azure, Salesforce, Google, and more.               |
| 🧑‍🤝‍🧑 **External Identities** | Secure collaboration with guests, partners, and customers.                  |

---

## 🏢 Common Use Cases

- ✅ Secure **remote access** for employees.
- ✅ Manage **access to cloud/on-prem applications**.
- ✅ Maintain **compliance** with audit logs and access reviews.
- ✅ Simplify **user and group management** with automation.

---

## 📚 Learn More

- 🔗 [Microsoft Entra ID Docs](https://learn.microsoft.com/en-us/entra/identity/)
- 🔗 [What is Entra ID?](https://learn.microsoft.com/en-us/entra/fundamentals/whatis)
- 🔗 [Microsoft Entra Product Page](https://www.microsoft.com/en-us/security/business/identity-access/microsoft-entra-id)

---



## 💡 Why Entra ID? Here's What Makes It a Game-Changer:

- 🔑 One Login for Everything – Say goodbye to juggling passwords.
- 🛡️ Stronger Security – MFA, passwordless login, real-time risk checks.
- 🧠 Centralized Management – Manage users, groups, and roles from one place.
- 🔄 Seamless Integration – Works with Microsoft apps & 3rd-party tools like Google, AWS, Salesforce.

## 🛠️ Key Admin Features:

- 👥 User & Device Management – Sync with on-prem AD & manage cloud identities.
- 🔐 Authentication Choices – Windows Hello 👁️, FIDO2 keys 🔑, mobile auth 📱.
- 🌍 Conditional Access – Grant access based on risk, location, & device health.
- 🧩 Dynamic Groups – Auto-assign users based on profile properties.
- 🎯 RBAC (Role-Based Access Control) – Give the right access to the right people 🔍.

## 💻 Device Management Integration:

- 📲 Real-Time Risk Assessments during sign-in.
- 🔁 Entra Join + SSO = Smooth user experience across all apps.
- 🧰 Intune Integration – Full device lifecycle management from one platform.

### 🔐 Microsoft Entra ID – License Overview

| **License**   | **Best For**             | **Key Focus**                                 |
|---------------|--------------------------|------------------------------------------------|
| **Free**      | Startups, small orgs     | Basic SSO, Microsoft 365                      |
| **P1**        | Most orgs                | Hybrid identity + Conditional Access          |
| **P2**        | Enterprises              | Advanced risk-based access + PIM              |
| **Governance**| Regulated sectors        | Deep governance + compliance                  |

# 💻 Microsoft Intune - Interview Preparation Guide

## 🎯 Interview Topics & Questions

### 1️⃣ What is Microsoft Intune?
**Answer:**  
Microsoft Intune is a cloud-based endpoint management solution that helps organizations manage and secure devices and apps. It integrates tightly with Entra ID and supports both MDM and MAM.

### 🚀 Key Features of Microsoft Intune

- 📱 Mobile Device Management (MDM) and Mobile Application Management (MAM)
- 🔐 Integration with Microsoft Entra ID (formerly Azure AD)
- 💼 Supports Windows, Android, iOS, macOS
- 🔁 Conditional Access Policies
- 🧰 Configuration Profiles (like Group Policies)
- 🦾 Compliance Policies
- 📦 Application Deployment (MSI, EXE, Store Apps, Web Apps)
- 🛡️ Endpoint Security via Defender for Endpoint
- 🔧 Windows Autopilot for Out-of-Box Setup
- 🔍 Monitoring and Reporting Dashboard
- 🔗 Integration with Microsoft Defender and other Microsoft 365 tools
### 2️⃣ What platforms does Intune support?
**Answer:**  
- Windows 10/11
- Android
- iOS/iPadOS
- macOS

---

### 3️⃣ What are Compliance Policies in Intune?
**Answer:**  
These define the rules and settings that a device must comply with to be considered secure. E.g., require BitLocker, block rooted devices, enforce password complexity.

---

### 4️⃣ What is the difference between Configuration Profiles and Compliance Policies?
**Answer:**  
- **Configuration Profiles**: Apply settings to devices (like Wi-Fi, certificates, restrictions).
- **Compliance Policies**: Assess whether a device meets security standards.

---

### 5️⃣ What is Conditional Access?
**Answer:**  
Conditional Access uses signals like device compliance, location, risk to grant/deny access to apps.

---

### 6️⃣ What is Windows Autopilot?
**Answer:**  
A deployment tool for pre-configuring and auto-enrolling devices into Intune with a customized Out-of-Box Experience (OOBE).

---

### 7️⃣ How does Intune handle app deployment?
**Answer:**  
Admins can push apps from:
- Microsoft Store
- Line-of-Business (LOB)
- Web links
- Win32 apps via Intune Management Extension

---

### 8️⃣ How do you monitor devices in Intune?
**Answer:**  
Via the Intune admin center dashboard showing device compliance, configuration status, deployment status, and endpoint protection alerts.

---

## 📘 Resources

- [Microsoft Learn - Intune](https://learn.microsoft.com/en-us/mem/intune/)
- [Windows Autopilot Overview](https://learn.microsoft.com/en-us/mem/autopilot/)
- [Intune on GitHub](https://github.com/Microsoft/Microsoft-Intune-Samples)

---

## 📋 Microsoft Intune Licensing Overview

| 🪪 **License**                  | 🧩 **Best For**                 | 🎯 **Key Features / Focus**                                                             |
|-------------------------------|--------------------------------|------------------------------------------------------------------------------------------|
| 🆓 **Free / Included**         | Startups, Small Teams          | Basic SSO, Microsoft 365 management, limited mobile device management (MDM)             |
| 🔐 **Intune Plan 1 (P1)**      | Most Organizations             | Conditional Access, MDM + MAM, Configuration Profiles, Compliance Policies              |
| 🚨 **Intune Plan 2 (P2)**      | Enterprises                    | Advanced Endpoint Security, Microsoft Defender for Endpoint, Risk-Based Access          |
| 🏛️ **Intune Suite / Add-ons**  | Regulated/Complex Environments | Remote Help, Endpoint Privilege Management, Advanced Analytics, Microsoft Tunnel for MAM |


## 👏 Final Note
Star 🌟 this repo if it helped and feel free to contribute by opening a PR!

---



# 🧰 PowerShell Basic Commands for Wintel Administrators

A handy **PowerShell command reference** for Windows Server (Wintel) administrators.  
Use these commands for daily management, troubleshooting, and automation.


## 🖥️ System Information

```powershell
# Get detailed system information
Get-ComputerInfo

# Basic computer system info
Get-WmiObject Win32_ComputerSystem

# Check OS version
(Get-WmiObject Win32_OperatingSystem).Caption

# Get list of running processes
Get-Process

# Get list of running services
Get-Service

# Restart or shutdown the system
Restart-Computer
Stop-Computer
```

---

## 🌐 Network Commands

```powershell
# Get IP configuration
Get-NetIPAddress

# Show network adapters
Get-NetAdapter

# Test network connectivity (Ping equivalent)
Test-Connection google.com

# Test specific port connectivity
Test-NetConnection -ComputerName google.com -Port 443

# Display routing table
Get-NetRoute
```

---

## 🔐 Active Directory (AD) Commands

> 🧩 Requires RSAT / ActiveDirectory module installed.

```powershell
# Import Active Directory module
Import-Module ActiveDirectory

# Get user information
Get-ADUser -Identity jdoe

# Search for all users and display key info
Get-ADUser -Filter * | Select Name, SamAccountName

# Get group members
Get-ADGroupMember -Identity "Domain Admins"

# Reset a user password
Set-ADAccountPassword -Identity jdoe

# Unlock a user account
Unlock-ADAccount -Identity jdoe
```

---

## 💾 File System Management

```powershell
# List files in a directory
Get-ChildItem C:\Logs

# Copy a file or folder
Copy-Item C:\file.txt D:\Backup\

# Move a file
Move-Item C:\file.txt D:\Archive\

# Delete files or folders
Remove-Item C:\Temp\* -Recurse -Force

# Get file or folder properties
Get-ItemProperty C:\file.txt
```

---

## 🧑‍💻 User & Process Management

```powershell
# List local users
Get-LocalUser

# Create a new local user
New-LocalUser -Name "testuser" -Password (Read-Host -AsSecureString)

# List running processes (sorted by CPU usage)
Get-Process | Sort-Object CPU -Descending

# Kill a process by name
Stop-Process -Name notepad -Force
```

---

## 💽 Disk & Storage Management

```powershell
# List all volumes
Get-Volume

# Show physical disk details
Get-Disk

# List all partitions
Get-Partition

# Show logical drives
Get-PSDrive
```

---

## 🧩 RDP and Port Checks

```powershell
# Test RDP (port 3389)
Test-NetConnection -ComputerName Server01 -Port 3389

# Check if port is listening locally
netstat -an | find "3389"
```

---

## ⚙️ Common Parameters and Switches

| Switch     | Description                                |
| ---------- | ------------------------------------------ |
| `-Force`   | Override restrictions or confirmations     |
| `-Recurse` | Include all child items and subfolders     |
| `-Confirm` | Prompt before executing                    |
| `-WhatIf`  | Show what would happen (without executing) |
| `-Verbose` | Display detailed command output            |

**Example:**

```powershell
Remove-Item C:\Temp\* -Recurse -WhatIf
```

---

## 📘 Help & Documentation

```powershell
# Get help for a cmdlet
Get-Help Get-Service

# Show examples only
Get-Help Get-Service -Examples

# Display full syntax and parameters
Get-Help Get-Service -Full
```

---

## ⚡ Common Server Administration Tasks

```powershell
# Restart a remote computer
Restart-Computer -ComputerName Server01 -Force

# Get stopped services on a remote server
Get-Service -ComputerName Server01 | Where-Object {$_.Status -eq "Stopped"}

# Export process list to CSV
Get-Process | Export-Csv C:\Reports\Processes.csv -NoTypeInformation
```
Sure 👍 — here are your sentences **corrected** with proper grammar and clarity, along with quick **PowerShell examples** for each so you can add them to your notes or GitHub doc.

---

### ✅ **Corrected Sentences + Examples**

---

### 1️⃣ **How to create an AD user in PowerShell**

✅ **Correct sentence:**

> How to create an Active Directory (AD) user in PowerShell?

**Example:**

```powershell
# Import AD module
Import-Module ActiveDirectory

# Create a new AD user
New-ADUser -Name "John Doe" `
           -SamAccountName jdoe `
           -UserPrincipalName jdoe@domain.com `
           -Path "OU=Users,DC=domain,DC=com" `
           -AccountPassword (Read-Host -AsSecureString "Enter Password") `
           -Enabled $true
```

---

### 2️⃣ **How to check the latest PowerShell path installed**

✅ **Correct sentence:**

> How to check the latest PowerShell installation path?

**Example:**

```powershell
# Show path of the current PowerShell executable
$PSHOME

# Or get version and path info
$PSVersionTable.PSVersion
$PSHOME
```

**Output Example:**

```
Major  Minor  Build  Revision
-----  -----  -----  --------
7      5      1      0
C:\Program Files\PowerShell\7
```

---

### 3️⃣ **How to check disk space in PowerShell**

✅ **Correct sentence:**

> How to check disk space using PowerShell?

**Example:**

```powershell
# Get disk usage and free space
Get-PSDrive -PSProvider FileSystem

# Or detailed info
Get-WmiObject Win32_LogicalDisk | Select-Object DeviceID, VolumeName, @{Name='FreeGB';Expression={"{0:N2}" -f ($_.FreeSpace/1GB)}}, @{Name='TotalGB';Expression={"{0:N2}" -f ($_.Size/1GB)}}
```

---

### 4️⃣ **How to check event logs in PowerShell**

✅ **Correct sentence:**

> How to check event logs using PowerShell?

**Example:**

```powershell
# List available event logs
Get-EventLog -List

# Show the latest 10 System log entries
Get-EventLog -LogName System -Newest 10

# Check for specific errors
Get-EventLog -LogName Application -EntryType Error -Newest 20
```

---

Would you like me to format these four sections into a **GitHub-ready Markdown block** (like your earlier Wintel README style)?
I can align and style it for your documentation.


## 🧾 Author

**Manikanta Suru**  
*Wintel Administrator | PowerShell Enthusiast*


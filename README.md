⚡ Windows PowerShell Fundamentals – Hands-On Lab
📘 Overview

This repository documents my hands-on learning and practical use of Windows PowerShell through a TryHackMe lab environment focusing on understanding how PowerShell is used in real-world environments, particularly within system administration, cybersecurity operations, and incident response.
PowerShell is a powerful task automation and configuration management framework built on the .NET platform. Unlike traditional text-based command-line tools, PowerShell is object-oriented, allowing administrators and security professionals to work with structured data, automate complex tasks, and manage systems at scale.

🧠 Why PowerShell Matters
PowerShell is a core skill across modern IT and cybersecurity roles because it enables:
Automation of repetitive administrative tasks
Deep visibility into system and network configuration
Object-based data manipulation instead of raw text parsing

Remote system management at scale
Efficient investigation during security incidents
PowerShell is heavily used by defenders and attackers alike, making it critical to understand from both perspectives.

🧩 Lab Environment
Platform: TryHackMe
Target OS: Windows Server
Shell: Windows PowerShell
Access Method: Command Prompt → PowerShell
Tools Used:
Built-in PowerShell cmdlets
PowerShell Help System
Object-based pipelines

🧱 PowerShell Fundamentals
Cmdlets and Syntax
PowerShell commands, known as cmdlets, follow a consistent Verb-Noun structure:
Get-Content
Set-Location
New-Item
This naming convention improves readability and discoverability.
Key discovery and learning cmdlets:
Get-Command – lists available cmdlets, functions, and scripts
Get-Help – provides usage details, parameters, and examples
Get-Alias – maps traditional commands (e.g., dir, cd) to PowerShell equivalents

📂 File System Navigation & Management
I practiced managing files and directories using PowerShell-native cmdlets:
Get-ChildItem – list files and directories
Set-Location – change directories
New-Item – create files and directories
Remove-Item – delete files and directories
Copy-Item and Move-Item – manage files and folders
Get-Content – read file contents
PowerShell simplifies file operations by using a single, consistent set of cmdlets rather than separate commands for files and directories.

🔗 Object-Based Piping & Filtering
PowerShell pipelines pass objects, not plain text. This enables powerful data manipulation without parsing strings.
Key filtering and transformation cmdlets:
Where-Object – filter objects based on conditions
Select-Object – select properties or limit output
Sort-Object – sort objects by properties
Select-String – search for patterns within files (similar to grep)
Common comparison operators used:
-eq, -ne
-gt, -ge
-lt, -le
-like
This object-based model allows complex command chains to be built efficiently and readably.

🖥️ System & Network Enumeration
I used PowerShell to gather detailed system and network information, including:
Get-ComputerInfo – comprehensive system configuration
Get-LocalUser – enumerate local user accounts
Get-NetIPConfiguration – network interface details
Get-NetIPAddress – assigned IP addresses
Compared to legacy tools, these cmdlets provide richer and more structured output, which is especially useful for automation and investigations.

⚙️ Process, Service, and Connection Analysis
To monitor dynamic system activity, I explored:
Get-Process – running processes with resource usage
Get-Service – service status and configuration
Get-NetTCPConnection – active TCP connections
These cmdlets are highly valuable during:
Incident response
Malware analysis
Threat hunting
System troubleshooting
I also reviewed Get-FileHash for file integrety verification and discussed Alternate Data Streams (ADS) as a persistence and stealth technique used by attackers.

🧠 PowerShell Scripting & Automation Concepts
While full scripting was beyond the scope of this lab, I explored how PowerShell scripting enables:
Automation of administrative tasks
Log analysis and IOC extraction
System integrity checks
Security monitoring and response automation
PowerShell scripting is widely used across:
Blue team operations (IR, SOC, threat hunting)
Red team activities (enumeration, payload execution, obfuscation)
System administration and configuration management
🌐 Remote Command Execution
I studied the Invoke-Command cmdlet, which allows commands or scripts to be executed on remote systems.
Key takeaways:
Enables centralized management of multiple machines
Can execute inline commands using -ScriptBlock
Commonly used by administrators, security engineers, and attackers
Understanding Invoke-Command is essential for both secure remote administration and detecting malicious lateral movement.

🛡️ Security Takeaways
PowerShell provides deep visibility into Windows systems
Object-based pipelines enable powerful automation and analysis
Many real-world attacks leverage PowerShell for stealth and control
Monitoring PowerShell activity is critical in enterprise environments
Strong PowerShell fundamentals improve detection and response capabilities

📌 Why This Matters for Cybersecurity
This project demonstrates practical PowerShell knowledge relevant to:
SOC analysis
Incident response
Threat hunting
Malware analysis
Enterprise system administration
PowerShell proficiency is a foundational skill for defending modern Windows environments.

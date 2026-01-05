# Windows Internals

## Overview
This document contains notes from Windows Fundamentals 2 (TryHackMe).
It focuses on internal Windows components such as services, registry,
startup processes, and system configuration tools.

---

## Windows Services
- Services are background processes managed by the Service Control Manager (SCM)
- Each service has a display name and an internal service name
- Services can start automatically, manually, or be disabled
- Sysmon is a Sysinternals service used for system monitoring and logging

---

## Sysmon
- Sysmon (System Monitor) is part of Microsoft Sysinternals
- Provides detailed logs about:
  - Process creation
  - Network connections
  - File creation and modification
- Commonly used by SOC analysts and blue team for detection and forensics

---

## Windows Registry
- Central database for system and application settings
- Contains configuration for:
  - Users
  - Services
  - Startup programs
- Incorrect registry changes can cause system instability

---

## Startup Applications
- Programs that run automatically at system boot
- Can be managed via:
  - Task Manager
  - Registry
  - System Configuration (msconfig)
- Malware often abuses startup locations for persistence

---

## System Configuration (msconfig)
- Provides access to advanced troubleshooting tools
- Includes networking diagnostics such as:
  - C:\Windows\System32\cmd.exe /k ipconfig /all
- Useful for diagnosing boot and service-related issues

---

## Security Considerations
- Principle of least privilege applies to services and users
- Monitoring services helps detect malicious persistence
- Understanding startup locations is essential for incident response

---

## Common Errors
- Confusing display names with service names
- Disabling critical services without understanding their function
- Modifying the registry without backups
- Ignoring startup programs when investigating malware

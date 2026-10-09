# Red Team Tools
<div align="center" style="margin: 30px 0;">

**A curated list of red teaming tools, C2 frameworks, and adversary simulation resources - organized by kill chain phase for offensive security professionals, penetration testers, and purple teamers.**

> **Disclaimer:** This repository is intended for authorized security testing, educational purposes, and adversary simulation only. The maintainers are not responsible for any misuse of the tools listed here. Always obtain proper written authorization before testing any system you do not own.

![Hacking Anime](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExYzJ4ZXNjb2Z6cHdqMGgyczFpZGxsYWxveHlxMWNwZG5pZWE1NnpmNyZlcD12MV9naWZzX3NlYXJjaCZjdD1n/VbEloWwOz3QqYBsqIZ/giphy.gif)
</div>
<br>

---

## About

This is a categorized collection of offensive security tools used across the full red team kill chain - from initial access and execution to persistence, privilege escalation, defense evasion, credential access, discovery, lateral movement, collection, command & control, and exfiltration.

Whether you're a red teamer, penetration tester, purple teamer, or security researcher, this list aims to be a single reference for the modern offensive toolkit.

---

## Table of Contents

- [🎯 Initial Access](#-initial-access)
- [⚙️ Execution](#️-execution)
- [🔒 Persistence](#-persistence)
- [🔼 Privilege Escalation](#-privilege-escalation)
- [🛡️ Defense Evasion](#️-defense-evasion)
- [🔑 Credential Access](#-credential-access)
- [🔍 Discovery](#-discovery)
- [🚀 Lateral Movement](#-lateral-movement)
- [📦 Collection](#-collection)
- [📡 Command & Control (C2)](#-command--control-c2)
- [📤 Exfiltration](#-exfiltration)
- [🌐 Web Exploitation](#-web-exploitation)
- [☁️ Cloud & Container Attacks](#️-cloud--container-attacks)
- [🧠 Active Directory Attacks](#-active-directory-attacks)
- [📱 Mobile & IoT Red Teaming](#-mobile--iot-red-teaming)
- [🎭 Social Engineering](#-social-engineering)
- [🧰 Payload Development & Obfuscation](#-payload-development--obfuscation)
- [🔬 Labs & Practice Environments](#-labs--practice-environments)
- [🧩 Miscellaneous](#-miscellaneous)

---

## Initial Access

- 🎣 **[Gophish](https://getgophish.com/)** - Open-source phishing framework for creating, launching, and tracking simulated phishing campaigns and credential capture exercises.
- 🪤 **[Evilginx2](https://github.com/kgretzky/evilginx2)** - Man-in-the-middle phishing proxy framework for capturing credentials and session cookies, bypassing two-factor authentication.
- 📧 **[King Phisher](https://github.com/rsmusllp/king-phisher)** - Phishing campaign toolkit designed for testing and promoting user awareness through realistic attack simulations.
- 🎯 **[SET (Social-Engineer Toolkit)](https://github.com/trustedsec/social-engineer-toolkit)** - Advanced framework for social engineering attacks, including spear-phishing, website cloning, and infectious media generation.
- 📦 **[Erebus](https://github.com/Improper-Input/erebus)** - Initial Access wrapper for the Mythic C2 framework that converts shellcode into payloads tailored for phishing and initial access operations.
- 🕵️ **[W.A.L.K. (WebAssembly Lure Krafter)](https://github.com/JumpsecLabs/WALK_WebAssembly_Lure_Krafter)** - WebAssembly (WASM) phishing lure generator for leveraging WASM smuggling techniques during red team exercises.
- 📲 **[iShelly](https://github.com/AutomoxSecurity/iShelly)** - Tool for generating macOS initial access vectors using Prelude Operator payloads.
- 📄 **[RTI-Toolkit](https://github.com/nickvourd/RTI-Toolkit)** - Remote Template Injection Toolkit for weaponizing Microsoft Office documents for initial access.
- 🦠 **[HTAC2](https://github.com/TREXNEGRO/HTAC2)** - Cloudflare-tunneled HTA (HTML Application) initial access stager with no persistent infrastructure requirements.
- 🖼️ **[ShadowPhish](https://github.com/baohuiking/ShadowPhish)** - APT awareness toolkit with phishing site templates, malicious LNK builders, HTML smuggling, and QR code phishing generators.

---

## Execution

- 🐚 **[PowerSploit](https://github.com/PowerShellMafia/PowerSploit)** - Collection of PowerShell modules for offensive security, covering code execution, persistence, and credential theft with in-memory execution to evade AV.
- 🎯 **[Metasploit Framework](https://www.metasploit.com/)** - Leading penetration testing framework for developing, testing, and executing exploit code, with Meterpreter for advanced post-exploitation control.
- 🪟 **[CrackMapExec](https://github.com/byt3bl33d3r/CrackMapExec)** - Swiss army knife for pentesting Windows/Active Directory networks, enabling command execution across multiple hosts via SMB, WMI, and WinRM.
- ⚡ **[Impacket](https://github.com/fortra/impacket)** - Python toolkit for working with network protocols, providing tools for remote command execution via PsExec, WMI, DCOM, and SMB.
- 🔧 **[PsExec](https://learn.microsoft.com/en-us/sysinternals/downloads/psexec)** - Lightweight telnet replacement that executes processes on remote systems, widely used for lateral movement and remote execution.
- 🖥️ **[PowerLessShell](https://github.com/Mr-Un1k0d3r/PowerLessShell)** - Executes PowerShell scripts and commands via MSBuild.exe without spawning powershell.exe, evading detection.
- 🐍 **[Nishang](https://github.com/samratashok/nishang)** - Framework of PowerShell scripts and payloads for all phases of penetration testing, with a focus on stealthy execution.
- 🔌 **[WMIOps](https://github.com/ChrisTruncer/WMIOps)** - PowerShell script leveraging WMI for remote command execution and system actions within Windows environments.
- 📡 **[Atomic Red Team](https://github.com/redcanaryco/atomic-red-team)** - Library of small, testable attack simulations mapped to MITRE ATT&CK, enabling execution technique validation.
- 🐚 **[Covenant](https://github.com/cobbr/Covenant)** - .NET command and control framework designed for collaborative red teaming with emphasis on offensive .NET tradecraft.

---

## Persistence

- 🩸 **[SharpGPOAbuse](https://github.com/FSecureLABS/SharpGPOAbuse)** - .NET tool that exploits edit rights on Group Policy Objects (GPOs) to compromise controlled objects and establish persistence across domain-joined systems.
- 🏗️ **[SharpStay](https://github.com/0xthirteen/SharpStay)** - .NET project for installing various persistence mechanisms on Windows systems, designed for red team operations.
- 🎯 **[StayKit](https://github.com/0xthirteen/StayKit)** - Cobalt Strike kit providing persistence capabilities through the Beacon payload, enabling long-term access maintenance.
- 🪟 **[Phantom Persistence (Rust)](https://github.com/Teach2Breach/phantom_persist_rs)** - Rust implementation of a persistence technique that hijacks the Windows shutdown process to restart applications without registry writes or elevated privileges.
- 🔧 **[Bitsadmin](https://lolbas-project.github.io/lolbas/Binaries/Bitsadmin/)** - Windows LOLBin that can create background transfer jobs executing payloads from Alternate Data Streams, usable for stealthy persistence.
- 📜 **[Cscript](https://lolbas-project.github.io/lolbas/Binaries/Cscript/)** - Windows script host binary that can execute VBS scripts stored in Alternate Data Streams, useful for hiding persistence mechanisms.
- 🔄 **[Runonce](https://lolbas-project.github.io/lolbas/Binaries/Runonce/)** - Windows LOLBin that executes Run Once tasks configured in the registry, including via Active Setup for persistence.
- 🖥️ **[WorkFolders](https://lolbas-project.github.io/lolbas/Binaries/WorkFolders/)** - Windows binary that can achieve proxy execution and persistence via App Paths registry hijacking.
- 🛡️ **[OfflineScannerShell](https://lolbas-project.github.io/lolbas/Binaries/OfflineScannerShell/)** - Windows Defender Offline Shell that executes mpclient.dll from the current working directory, exploitable for persistence.
- 🔗 **[SettingSyncHost](https://lolbas-project.github.io/lolbas/Binaries/SettingSyncHost/)** - Windows host process that can execute arbitrary batch scripts in the background without a window, usable for stealthy persistence.

---

## Privilege Escalation

- 🥔 **[DeadPotato](https://github.com/lypd0/DeadPotato)** - Windows privilege escalation utility from the Potato family that leverages SeImpersonatePrivilege to obtain SYSTEM privileges, with modules for command execution, reverse shells, SAM dumping, and BloodHound collection.
- 🍟 **[JuicyPotato](https://github.com/ohpe/juicy-potato)** - Local privilege escalation tool that abuses token impersonation via SeImpersonatePrivilege, widely used in IIS and MS-SQL environments to elevate service accounts to SYSTEM.
- 🐕 **[PowerSploit](https://github.com/PowerShellMafia/PowerSploit)** - PowerShell post-exploitation framework whose PowerUp module identifies and exploits local privilege escalation opportunities including DLL hijacking and service misconfigurations.
- 🩸 **[bloodyAD](https://github.com/CravateRouge/bloodyAD)** - Active Directory privilege escalation Swiss army knife that performs LDAP-based privesc operations using cleartext, pass-the-hash, or certificate authentication.
- 🔍 **[PrivescCheck](https://github.com/itm4n/PrivescCheck)** - PowerShell enumeration script for Windows that audits common privilege escalation misconfigurations without performing exploitation, outputting potential escalation paths.
- 🐧 **[LinPEAS](https://github.com/peass-ng/PEASS-ng)** - Comprehensive Linux privilege escalation enumeration script that scans for misconfigured sudo rules, writable paths, SUID/SGID binaries, kernel vulnerabilities, and service weaknesses.
- 🪟 **[WinPEAS](https://github.com/peass-ng/PEASS-ng)** - Windows counterpart to LinPEAS, automating discovery of privilege escalation vectors including weak service permissions, unquoted service paths, and registry misconfigurations.
- 🎯 **[BeRoot](https://github.com/AlessandroZ/BeRoot)** - Cross-platform post-exploitation tool that checks common misconfigurations on Windows, Linux, and macOS to identify privilege escalation vectors without performing exploitation.
- 🧬 **[ADAIO](https://github.com/BEND0US/ADAIO)** - Standalone Active Directory enumeration tool focused on identifying privilege escalation primitives including dangerous ACLs, ADCS ESC vulnerabilities, delegation attacks, and DCSync rights.
- 📦 **[KrbRelayUp](https://github.com/Dec0ne/KrbRelayUp)** - Universal local privilege escalation tool for domain environments where LDAP signing is not enforced, relaying Kerberos authentication from DCOM connections.

---

## Defense Evasion

- 🧬 **[ScareCrow](https://github.com/optiv/ScareCrow)** - Payload generation framework that produces DLL side-loading, ETW/AMSI patching, and syscall-based shellcode execution artifacts to evade endpoint detection.
- 🎭 **[Magnetar](https://github.com/magicsword-io/Magnetar)** - Feature-rich shellcode loader implementing direct syscalls, ETW/AMSI patching, Early Bird APC injection, and process protection via security descriptor modification.
- 🔇 **[EvtMute](https://github.com/boku7/EvtMute)** - Applies YARA-like filters to the Windows Event Log pipeline before events are written, allowing selective suppression of telemetry without clearing logs.
- 🕵️ **[Phant0m](https://github.com/hlldz/Phant0m)** - Technique that locates and kills Event Log service threads instead of clearing logs, avoiding the canonical event 1102 indicator associated with log deletion.
- 🔌 **[BOF-patchit](https://github.com/rsmudge/BOF-patchit)** - All-in-one Cobalt Strike Beacon Object File to patch, check, and revert AMSI and ETW in memory, leaving no disk artifacts for forensic analysis.
- 🧹 **[SigFlip](https://github.com/med0x2e/SigFlip)** - Tool for patching Authenticode-signed PE files (exe, dll, sys) without invalidating or breaking the existing digital signature, enabling payload injection into signed binaries.
- 📦 **[Donut](https://github.com/TheWover/donut)** - Generates position-independent shellcode from .NET assemblies, VBScript, JScript, and other Windows payloads for in-memory execution, avoiding disk-based detection.
- 🌫️ **[Havoc](https://github.com/HavocFramework/Havoc)** - Modern C2 framework with built-in sleep obfuscation (Ekko), return address spoofing, indirect syscalls, and stack spoofing for evading memory scanners and behavioral detection.
- 🐍 **[Sliver](https://github.com/BishopFox/sliver)** - Cross-platform implant framework supporting JA3/JA4S fingerprint randomization, session migration, and multiple transport protocols to blend network traffic with legitimate activity.
- 🛡️ **[EDRChoker](https://github.com/TwoSevenOneT/EDRChoker)** - Throttles EDR telemetry by leveraging Windows QoS policies, requiring no process injection, driver loading, or suspicious memory operations to blind endpoint sensors.

---

## Credential Access

- 🍖 **[Mimikatz](https://github.com/gentilkiwi/mimikatz)** - The reference tool for Windows credential extraction, capable of dumping plaintext passwords, hashes, PINs, and Kerberos tickets from LSASS memory, LSA service, SAM database, and cached credentials.
- 🩸 **[GhostPack (SharpDPAPI, SafetyKatz, KeeThief)](https://github.com/GhostPack)** - Collection of C# offensive tools including SharpDPAPI for DPAPI secret extraction, SafetyKatz for in-memory credential dumping, and KeeThief for KeePass master key extraction.
- 📦 **[Impacket (secretsdump.py)](https://github.com/fortra/impacket)** - Python toolkit whose secretsdump module performs remote credential dumping via SAM/SECURITY/SYSTEM registry extraction, NTDS.dit theft, and DCSync replication, supporting pass-the-hash and VSS methods.
- 🎟️ **[Rubeus](https://github.com/GhostPack/Rubeus)** - C# toolset for Kerberos abuse including Kerberoasting (extracting TGS hashes for offline cracking), AS-REP Roasting, ticket extraction from memory, and Golden/Silver/Diamond ticket forgery.
- 🌐 **[Responder](https://github.com/lgandx/Responder)** - LLMNR, NBT-NS, and mDNS poisoner that captures NetNTLMv1/v2 hashes by answering broadcast name resolution requests, enabling relay attacks and offline cracking.
- 🔑 **[dploot](https://github.com/zblurx/dploot)** - Python rewrite of SharpDPAPI that loots DPAPI-protected secrets locally or remotely, including browser credentials, certificates, vaults, masterkeys, and machine credentials.
- 🪟 **[Windows Credential Editor (WCE)](https://www.ampliasecurity.com/research/windows-credentials-editor/)** - Post-exploitation utility for dumping credentials from LSASS memory and local stores, historically used alongside Mimikatz for pass-the-hash and pass-the-ticket operations.
- 🔓 **[pyGoldenGMSA](https://github.com/felixbillieres/pyGoldenGMSA)** - Cross-platform Python implementation of the GoldenGMSA attack that computes Group Managed Service Account passwords offline from compromised KDS Root Keys.
- 🗄️ **[KeePwn](https://github.com/Orange-Cyberdefense/KeePwn)** - Python tool to automate KeePass database discovery and secret extraction across compromised environments.
- 🕵️ **[Atlas](https://github.com/portbuster1337/Atlas)** - Cross-platform C# Active Directory toolkit providing DCSync credential replication via MS-DRSR, SAM/LSA secret extraction through Remote Registry, and Kerberoasting/AS-REP Roasting modules.
- 🎯 **[ADscan](https://github.com/ADScanPro/adscan)** - All-in-one AD pentesting CLI that automates credential harvesting including SAM/LSA extraction, DCSync, Kerberoasting, AS-REP Roasting, and GPP password detection across a single workflow.
- 🐍 **[PPLBlade](https://github.com/TwoSevenOneT/PPLBlade)** - Protected Process Light dumper that bypasses PPL protection on LSASS and supports obfuscated, fileless memory dumps uploaded via RAW or SMB without writing to disk.

---

## Discovery

- 🩸 **[BloodHound](https://github.com/SpecterOps/BloodHound)** - Active Directory attack path mapping tool that ingests SharpHound data to visualize shortest paths to high-value targets, excessive privileges, and unconstrained delegation relationships.
- 🐕 **[SharpHound](https://github.com/SpecterOps/BloodHound/tree/main/src/SharpHound)** - C# data collector for BloodHound that enumerates users, groups, sessions, ACLs, trusts, and local admin rights across Active Directory environments.
- 🌐 **[Nmap](https://nmap.org/)** - The definitive network scanning and service discovery tool, used for host discovery, port scanning, OS fingerprinting, and vulnerability detection via NSE scripts.
- 🔌 **[NetExec](https://github.com/Pennyw0rth/NetExec)** - Swiss army knife for network enumeration that supports SMB, LDAP, WinRM, and MSSQL discovery of users, groups, shares, sessions, password policies, and logged-on users.
- 📊 **[Ladon](https://github.com/k8gege/Ladon)** - Large-scale intranet penetration scanner supporting 32 protocols for rapid asset discovery, including ICMP, SMB, WMI, SSH, HTTP, RDP, and more across batch A/B/C segment scanning.
- 🔍 **[enum4linux-ng](https://github.com/cddmp/enum4linux-ng)** - Next-generation Windows/Samba enumeration tool that extracts users, groups, shares, password policies, and OS information via RPC, SMB, and LDAP.
- 🏛️ **[Atlas](https://github.com/portbuster1337/Atlas)** - Cross-platform AD toolkit with modular discovery including SMB share/user/group enumeration, LDAP queries, Kerberos user enumeration, and BloodHound CE collection.
- 🎯 **[ADscan](https://github.com/ADScanPro/adscan)** - All-in-one AD pentesting CLI that automates LDAP, SMB, Kerberos, and DNS enumeration alongside attack-path graph collection in a single workflow.
- 📡 **[Aquattro](https://github.com/FranzAlvis/aquattro)** - Fast recon tool that takes IP lists and returns live hosts with screenshots and auto-generated HTML reports, supporting both Nmap-based full port discovery and web-focused scanning.
- 🧩 **[Brabus Recon Suite (BRS)](https://github.com/easypro-tech/brs)** - Professional toolkit for network reconnaissance featuring auto LAN discovery, port scanning via nmap/masscan, and system information auditing.

---

## Lateral Movement

- 🖥️ **[PsExec](https://learn.microsoft.com/en-us/sysinternals/downloads/psexec)** - Sysinternals utility that executes processes on remote systems via SMB by creating a temporary service, a cornerstone technique for Windows lateral movement.
- 🐍 **[Impacket (psexec.py / wmiexec.py / smbexec.py / atexec.py)](https://github.com/fortra/impacket)** - Python toolkit providing multiple remote execution methods: PsExec via SMB/SCM, WMI execution for stealthier operations, SMBExec for service-based execution, and AtExec for scheduled task execution.
- 🔧 **[CrackMapExec / NetExec](https://github.com/Pennyw0rth/NetExec)** - Swiss army knife for network pentesting that supports lateral movement via SMB, WMI, and WinRM across multiple hosts with `--exec-method` options.
- 📡 **[Evil-WinRM](https://github.com/Hackplayers/evil-winrm)** - WinRM shell that enables remote command execution over HTTP/HTTPS, supporting password, hash (pass-the-hash), and Kerberos authentication for lateral movement.
- 🎯 **[SharpSMBClient](https://github.com/0xthirteen/SharpSMBClient)** - C# SMB client for file operations and remote execution, useful for interacting with SMB shares during lateral movement.
- 🔄 **[mssqlproxy](https://github.com/blackarrowsec/mssqlproxy)** - Toolkit for lateral movement through compromised Microsoft SQL Server instances via socket reuse, enabling pivoting in restricted environments.
- 🛠️ **[MoveScheduler](https://github.com/mez-0/MoveScheduler)** - .NET tool for lateral movement using scheduled tasks, providing an alternative when other methods are blocked.
- 🖧 **[CSharpWinRM](https://github.com/mez-0/CSharpWinRM)** - .NET WinRM API implementation for remote command execution over WinRM, enabling lateral movement in Windows environments.
- 🔗 **[RDP Session Hijacking (tscon)](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/tscon)** - Abuse of Windows `tscon` utility as SYSTEM to attach to another user's existing RDP session without their password, including privileged sessions.
- 🚇 **[RDPWrapper](https://github.com/stascorp/rdpwrap)** - Tool that patches termsrv.dll to enable concurrent RDP sessions and hidden RDP access, abused by attackers for stealthy lateral movement.

---

## Collection

- 🎥 **[Pupy](https://github.com/n1nj4sec/pupy)** - Cross-platform RAT/backdoor framework with modules for keystroke capture, screenshot collection (including click-triggered mouse-logger captures), audio recording, and file exfiltration back to its C2 infrastructure.
- 📸 **[Auraboros](https://mallory.ai/malware/019db25f-4718-796a-b3e2-f97e51200c59)** - C2 framework supporting screenshot capture, webcam capture, live microphone/audio streaming, clipboard theft, keylogging, and browser credential/cookie/history extraction from Chrome and Brave.
- 🎤 **[FOOTWINE](https://github.com/alexander-hanel/APTnotes-md)** - APT37 malware with surveillance commands including screenshot capture, keystroke logging, audio capture, and video surveillance capabilities.
- 📱 **[Payload-FNROID](https://github.com/HLSV/payload-FNROID)** - Android payload generator for ethical testing that captures audio (microphone), screenshots, front-camera selfies, and system information collection.
- 🖼️ **[SharpScreenshot](https://github.com/GhostPack/SharpScreenshot)** - C# tool for capturing desktop screenshots on Windows systems, useful for visual intelligence collection during red team operations.
- 📋 **[ClipboardTool](https://github.com/0xthirteen/ClipboardTool)** - Tool for capturing and manipulating clipboard contents to collect passwords, cryptocurrency addresses, and other sensitive data copied by users.
- 🗂️ **[Seatbelt](https://github.com/GhostPack/Seatbelt)** - C# security-oriented host survey tool that collects comprehensive system information including user data, system configuration, and potentially sensitive files.
- 🎣 **[CuddlePhish](https://github.com/fkasler/cuddlephish)** - Browser session hijacking tool designed for collecting authenticated web session data and information from targeted applications.
- 📧 **[MailSniper](https://github.com/dafthack/MailSniper)** - PowerShell tool for searching through Exchange and Office 365 mailboxes to collect sensitive emails and attachments during red team engagements.
- 🗄️ **[AtlasReaper](https://github.com/mdsecactivebreach/AtlasReaper)** - Data collection tool for Confluence and Jira environments, enabling mining of information repositories for sensitive data.

---

## Command & Control (C2)

- 🎯 **[Cobalt Strike](https://www.cobaltstrike.com/)** - Industry-standard adversary simulation platform with the Beacon payload, featuring Malleable C2 profiles for traffic customization, SMB beacons for internal pivoting, and extensive post-exploitation capabilities including execute-assembly, process injection, and Mimikatz integration.
- 🐍 **[Sliver](https://github.com/BishopFox/sliver)** - Open-source cross-platform C2 framework supporting mTLS, WireGuard, HTTP(S), and DNS transports with procedurally generated C2 traffic and dynamically compiled implants with unique per-instance encryption keys.
- 🌫️ **[Havoc](https://github.com/HavocFramework/Havoc)** - Modern malleable post-exploitation C2 framework with a C/ASM agent called Demon, featuring sleep obfuscation via Ekko/FOLIAGE, indirect syscalls, x64 return address spoofing, and token vault capabilities.
- 🧩 **[Mythic](https://github.com/its-a-feature/Mythic)** - Modular, collaborative C2 platform with plug-and-play agent architecture, web-based React UI, GraphQL API, and built-in MITRE ATT&CK mapping for operational tracking and deconfliction.
- 🦡 **[Brute Ratel C4](https://bruteratel.com/)** - Commercial command and control framework with a "badger" agent that detects EDR userland hooks via built-in debugger, supports DNS over HTTPS, indirect syscalls, and can tunnel C2 through legitimate services like Microsoft Teams and Slack.
- 🔄 **[Covenant](https://github.com/cobbr/Covenant)** - .NET command and control framework designed for collaborative red teaming with a focus on offensive .NET tradecraft and modular grunt implants.

---

## Exfiltration

- 🐍 **[PyExfil](https://github.com/ytisf/PyExfil)** - Python toolkit for researching and stress-testing data exfiltration techniques across 20+ covert channels including DNS, ICMP, HTTPS, NTP, Slack, and QUIC, designed for DLP detection testing and red team simulation.
- 📦 **[Croc](https://github.com/schollz/croc)** - CLI file transfer tool with end-to-end encryption and support for private relays, allowing secure exfiltration of large files with flags to disable local broadcast traffic for operational stealth.
- 🌐 **[Mística](https://github.com/IncideDigital/Mistica)** - Covert channel tool that embeds data within application-layer protocols like HTTP and DNS using a custom SOTP (Simple Overlay Transport Protocol), encrypting and transmitting information in specific packet fields.
- 🕵️ **[DET (Data Exfiltration Toolkit)](https://github.com/sensepost/DET)** - Extensible data exfiltration toolkit supporting multiple channels including DNS, ICMP, and HTTP for red team operations and detection capability testing.
- 📡 **[DNSExfiltrator](https://github.com/Arno0x/DNSExfiltrator)** - Data leak testing tool that transfers files over a DNS request covert channel, encoding data in DNS queries to bypass traditional network monitoring.
- 🔐 **[PacketWhisper](https://github.com/TryCatchHCF/PacketWhisper)** - Stealthy exfiltration tool using DNS queries and text-based steganography to defeat attribution and bypass network detection controls.
- 🎯 **[ToRat](https://github.com/lu4p/ToRat)** - Remote administration tool that embeds a TOR instance in the binary, establishing covert side channels through the TOR network for exfiltration and communication.
- 🚀 **[VeilTransfer](https://github.com/infosecn1nja/VeilTransfer)** - Data exfiltration utility with DNS over HTTPS, QUIC, ICMP, and Dropbox-based transfer methods, plus scheduled transfer capabilities for operational control and detection evasion.
- 📥 **[Egress-Assess](https://github.com/ChrisTruncer/Egress-Assess)** - Tool for testing egress data detection capabilities, simulating data exfiltration across multiple protocols to evaluate DLP and network monitoring effectiveness.
- 📤 **[PowerShell RAT](https://github.com/Viralmaniar/Powershell-RAT)** - Python-based backdoor that uses Gmail to exfiltrate data as email attachments, blending exfiltration traffic with legitimate cloud service usage.

---

## Web Exploitation

- 🛡️ **[Burp Suite](https://portswigger.net/burp)** - Industry-standard web security testing platform with a complete suite of tools including proxy interception, automated DAST scanning, and extensive extensibility via the BApp Store.
- 🕷️ **[OWASP ZAP](https://www.zaproxy.org/download/)** - Open-source web application security scanner and proxy, ideal for automated DAST scanning and manual penetration testing with a growing marketplace of add-ons.
- 🐍 **[SQLmap](https://sqlmap.org/)** - Automated SQL injection detection and exploitation tool that supports a wide range of database backends and advanced techniques for database takeover.
- 🎯 **[Nuclei](https://github.com/projectdiscovery/nuclei)** - Fast vulnerability scanner powered by a vast library of community-contributed templates, enabling rapid identification of misconfigurations, CVEs, and exposed endpoints.
- 🐚 **[Commix](http://commixproject.com/)** - Automated command injection exploiter designed to detect and exploit OS command injection vulnerabilities in web-based applications.
- 🔍 **[Gobuster](https://github.com/OJ/gobuster)** - High-speed brute-force tool for discovering hidden directories, files, DNS subdomains, and virtual hosts on web servers.
- 🌀 **[ffuf](https://github.com/ffuf/ffuf)** - Fast web fuzzer written in Go, widely used for directory discovery, parameter fuzzing, and virtual host enumeration with flexible filtering options.
- ⚡ **[Feroxbuster](https://feroxbuster.com/)** - Rust-powered recursive content discovery tool that automatically scans newly found paths and extracts links for deeper enumeration.
- 🧪 **[XSStrike](https://github.com/s0md3v/XSStrike)** - Advanced XSS detection suite with intelligent payload generation, context analysis, and integrated fuzzing engine for crafting guaranteed working payloads.
- 🦊 **[Dalfox](https://github.com/hahwul/dalfox)** - Parameter analysis and XSS scanning tool that identifies injection points, analyzes reflected parameters, and detects bad-header configurations.
- 🎯 **[WPScan](https://wpscan.com/)** - WordPress-specific security scanner with a continuously updated database of core, plugin, and theme vulnerabilities, available as CLI and API.
- 🧩 **[JoomScan](https://github.com/rezasp/joomscan)** - OWASP Joomla vulnerability scanner that automates detection of known offensive vulnerabilities and misconfigurations in Joomla CMS deployments.
- 🕵️ **[Caido](https://www.caido.io/)** - Modern lightweight web security auditing toolkit designed as a faster alternative to Burp Suite, with a free tier and extensible plugin ecosystem.

---

## Cloud & Container Attacks

- 🔎 **[AzureHound](https://github.com/SpecterOps/AzureHound)** - Azure AD data collector that maps roles, group memberships, and privilege escalation paths into BloodHound for visualizing cloud identity attack paths.
- 🛣️ **[ROADtools](https://github.com/dirkjanm/roadtools)** - Azure AD/Entra ID attack suite supporting tenant enumeration, authentication, and token manipulation, including roadrecon, roadtx, and roadlib modules.
- 🛠️ **[AADInternals](https://github.com/Gerenios/AADInternals)** - PowerShell toolkit for deep Azure AD exploitation, covering token manipulation, federation backdoors, and mailbox manipulation for persistence testing in Microsoft 365 environments.
- 📊 **[GraphRunner](https://github.com/dafthack/GraphRunner)** - Microsoft Graph API post-exploitation toolkit for quickly querying Azure AD roles, permissions, and user data via PowerShell.
- ☁️ **[ScoutSuite](https://github.com/nccgroup/ScoutSuite)** - Multi-cloud security auditing tool that systematically reviews identity configurations and permission policies across AWS, Azure, GCP, and other cloud platforms.
- 🧩 **[MicroBurst](https://github.com/NetSPI/MicroBurst)** - Collection of Azure security assessment scripts covering role enumeration, credential dumping, and automated account abuse for cloud post-exploitation scenarios.
- 🐳 **[CDK](https://github.com/cdk-team/CDK)** - Container environment penetration testing toolkit supporting security assessment of Kubernetes, Docker, and Containerd, capable of container escape and cluster reconnaissance.
- 🕳️ **[DEEPCE](https://github.com/stealthcopter/deepce)** - Docker enumeration, privilege escalation, and container escape tool designed for security assessment from inside containers.
- ⚔️ **[Peirates](https://github.com/inguardians/peirates)** - Kubernetes penetration testing tool that assesses cluster security posture from an attacker's perspective, supporting token theft and service account abuse.
- 🔬 **[kdigger](https://github.com/quarkslab/kdigger)** - Kubernetes-focused container assessment and context discovery tool for environment probing during penetration tests.
- 🛡️ **[KubiScan](https://github.com/cyberark/KubiScan)** - Kubernetes cluster risky permission scanner that identifies dangerous configurations in roles, role bindings, and service accounts.
- 🧪 **[KubeHound](https://github.com/DataDog/KubeHound)** - Kubernetes attack path builder that discovers potential lateral movement and privilege escalation routes within clusters through graph analysis.

---

## Active Directory Attacks

- 🩸 **[BloodHound](https://github.com/SpecterOps/BloodHound)** - Active Directory attack path mapping tool that uses graph theory to reveal hidden privilege relationships and shortest paths to Domain Admin, with over 70% of environments containing exploitable paths from any authenticated user.
- 🐕 **[SharpHound](https://github.com/SpecterOps/SharpHound)** - C# data collector for BloodHound that enumerates users, groups, sessions, ACLs, trusts, and local admin rights across Active Directory environments.
- 🍖 **[Mimikatz](https://github.com/gentilkiwi/mimikatz)** - Reference tool for Windows credential extraction, capable of dumping plaintext passwords, hashes, PINs, and Kerberos tickets from LSASS memory for AD credential access.
- 🎟️ **[Rubeus](https://github.com/GhostPack/Rubeus)** - C# toolset for raw Kerberos interaction and abuse, supporting Kerberoasting, AS-REP Roasting, Pass-the-Ticket, and delegation attacks.
- 📦 **[Impacket](https://github.com/fortra/impacket)** - Python toolkit providing protocol-level AD attacks including GetUserSPNs for Kerberoasting, secretsdump for DCSync, and psexec/wmiexec for lateral movement.
- 🔧 **[NetExec (CrackMapExec)](https://github.com/Pennyw0rth/NetExec)** - Swiss army knife for AD pentesting enabling authentication, enumeration, credential dumping, and code execution across SMB, LDAP, WinRM, and MSSQL.
- 🔐 **[Certipy](https://github.com/ly4k/Certipy)** - ADCS exploitation tool for finding and abusing ESC1 through ESC15 certificate template vulnerabilities to escalate to Domain Admin.
- 🔗 **[Responder](https://github.com/lgandx/Responder)** - LLMNR/NBT-NS/mDNS poisoner that captures NetNTLMv2 hashes from broadcast name resolution requests, enabling relay attacks and offline cracking.
- 🎯 **[Kerbrute](https://github.com/ropnop/kerbrute)** - Kerberos-based user enumeration and password spraying tool that avoids account lockout by making one attempt per account per window.
- 🐍 **[Certipy](https://github.com/ly4k/Certipy)** - ADCS attack suite that identifies vulnerable certificate templates (ESC1-ESC15) and automates exploitation including ESC8 NTLM relay to enrollment endpoints.
- 🦊 **[PowerView](https://github.com/PowerShellMafia/PowerSploit/tree/master/Recon)** - PowerShell recon module for domain enumeration including users, groups, computers, GPOs, ACLs, shares, and trust relationships.
- 🧪 **[PurpleSharp](https://github.com/mvelazc0/PurpleSharp)** - Open-source C# adversary simulation tool that executes MITRE ATT&CK techniques within Windows Active Directory environments for detection engineering validation.
- 🛠️ **[Atlas](https://github.com/portbuster1337/Atlas)** - Cross-platform C# AD toolkit providing SMB/Kerberos/LDAP enumeration, DCSync credential replication, and BloodHound CE collection in a NetExec-style workflow.
- 🔎 **[PingCastle](https://github.com/netwrix/pingcastle)** - AD security auditing tool that produces a health score of the AD environment and identifies major misconfigurations.
- 🎯 **[ADscan](https://github.com/ADScanPro/adscan)** - All-in-one AD pentesting CLI automating LDAP, SMB, Kerberos, and DNS enumeration alongside attack-path graph collection and credential harvesting.
- 🧩 **[Snaffler](https://github.com/SnaffCon/Snaffler)** - AD credential discovery tool that finds sensitive files and credentials across accessible shares using color-coded scoring.

---

## Mobile & IoT Red Teaming

- 🐍 **[Frida](https://frida.re/)** - World-class dynamic instrumentation toolkit that injects scripts into black-box processes on Android, iOS, and other platforms, enabling function hooking, crypto API monitoring, and private app logic tracing without source code.
- 🔍 **[MobSF](https://mobsf.github.io/docs/)** - Automated all-in-one mobile application security assessment framework supporting static and dynamic analysis for Android, iOS, and Windows apps, widely regarded as the industry-standard open-source tool for mobile pentesting.
- 📱 **[Objection](https://github.com/sensepost/objection)** - Frida-powered runtime mobile exploration toolkit that inspects container filesystems, bypasses SSL pinning, dumps keychain data, and performs in-memory manipulation without requiring a jailbroken device.
- 🧲 **[GATTacker](https://github.com/securing/gattacker)** - BLE man-in-the-middle proxy tool that clones a legitimate device's GATT profile to create a malicious twin, intercepting and modifying GATT commands between mobile apps and IoT devices.
- 📡 **[Ubertooth One](https://github.com/greatscottgadgets/ubertooth)** - Open-source Bluetooth Low Energy (BLE) sniffing and analysis platform that captures BLE advertising packets to reveal device identities, exposed services, and cleartext transmitted data.
- 🔌 **[CC2531 Sniffer](https://github.com/homeassistant/zigbee2mqtt)** - Low-cost Zigbee sniffing tool that works with the KillerBee framework to capture and decrypt Zigbee network traffic, allowing command injection once network keys are obtained.
- 📻 **[HackRF One](https://greatscottgadgets.com/hackrf/)** - Low-cost Software Defined Radio (SDR) platform covering 1 MHz to 6 GHz, used for analyzing Zigbee, LoRa, Sub-GHz, and custom IoT wireless protocols.
- 🧰 **[KillerBee](https://github.com/riverloopsec/killerbee)** - Zigbee security testing framework providing tools for network discovery, traffic capture, data replay, and association flood denial-of-service attacks.
- 📶 **[Aircrack-ng](https://www.aircrack-ng.org/)** - Wireless network security auditing suite with tools for monitor mode configuration, packet capture, frame injection, and WEP/WPA/WPA2-PSK key cracking, applicable to IoT device Wi-Fi network access auditing.
- 🔑 **[Hashcat](https://hashcat.net/hashcat/)** - GPU-accelerated password recovery tool supporting high-speed offline cracking of hashes extracted from IoT device firmware or configuration files, with dictionary, mask, and hybrid attack modes.

---

## Social Engineering

- 🎯 **[SET (Social-Engineer Toolkit)](https://github.com/trustedsec/social-engineer-toolkit)** - Advanced open-source framework for social engineering attacks, including spear-phishing, website cloning, infectious media generation, and credential harvesting, widely used in red team engagements.
- 🪤 **[Evilginx2](https://github.com/kgretzky/evilginx2)** - Standalone man-in-the-middle attack framework using reverse proxy phishing to capture credentials and session cookies, capable of bypassing two-factor authentication.
- 📧 **[Gophish](https://getgophish.com/)** - Open-source phishing framework for creating, launching, and tracking simulated phishing campaigns and credential capture exercises, with a clean web UI for campaign management.
- 👑 **[King Phisher](https://github.com/rsmusllp/king-phisher)** - Phishing campaign toolkit designed for testing and promoting user awareness through realistic attack simulations, with support for email templates and credential harvesting.
- 🎣 **[Phishing Frenzy](https://github.com/pentestgeek/phishing-frenzy)** - Ruby on Rails phishing campaign automation platform that streamlines the creation and management of phishing engagements.
- 📩 **[HiddenEye](https://github.com/DarkSecDevelopers/HiddenEye)** - Modern phishing tool with advanced social engineering features, supporting site cloning and multiple tunneling options for credential capture.
- 🔥 **[BlackEye](https://github.com/thelinuxchoice/blackeye)** - Phishing tool with site cloning capabilities, offering 30+ pre-built templates for popular platforms to harvest credentials during awareness exercises.
- 🛜 **[Zphisher](https://github.com/htr-tech/zphisher)** - Advanced phishing tool with tunneling support, providing 30+ templates and automated credential capture for security awareness training.
- 📡 **[SocialFish](https://github.com/UndeadSec/SocialFish)** - Social engineering phishing framework with a web-based control panel, supporting multiple phishing templates and real-time credential capture.
- 🕵️ **[Weeman](https://github.com/evait-security/weeman)** - HTTP server-based phishing framework that clones legitimate websites and captures submitted credentials for red team social engineering operations.
- 📲 **[QRGen](https://github.com/aravind0x7/QRGen)** - QR code phishing (quishing) generator that creates malicious QR codes redirecting victims to credential harvesting pages.
- 🐍 **[PyPhisher](https://github.com/KasRoudra/PyPhisher)** - Python-based phishing toolkit with multiple site templates and built-in tunneling support for credential harvesting campaigns.
- 🎯 **[SocialBox](https://github.com/Cyb3rWard0g/SocialBox)** - Brute-force social media hacking toolkit for testing account security across platforms like Facebook, Instagram, and Twitter.
- 🌐 **[CredSniper](https://github.com/ustayready/CredSniper)** - Phishing framework with two-factor authentication bypass support, enabling realistic credential harvesting against protected accounts.
- 🪝 **[Modlishka](https://github.com/drk1wi/Modlishka)** - Reverse proxy phishing framework that sits between the victim and legitimate website, capturing credentials and session tokens while transparently relaying traffic.

---

## Payload Development & Obfuscation

- 🍩 **[Donut](https://github.com/TheWover/donut)** - Position-independent shellcode generator that converts .NET assemblies, EXE/DLL files, and scripts into in-memory payloads, featuring encryption, compression, and remote staging via HTTP or DNS.
- 🧬 **[Fritter](https://github.com/0xROOTPLS/Fritter)** - Heavily modified Donut fork producing fully polymorphic shellcode with rewritten crypto, compression, and API resolution layers, plus dynamic memory permissions using VEH sliding window execution.
- 🪶 **[Veil-Evasion](https://github.com/Veil-Framework/Veil-Evasion)** - Payload generation framework that transforms scripts into standalone native binaries using template-based source injection, designed to bypass common antivirus solutions.
- 🐍 **[ScareCrow](https://github.com/optiv/ScareCrow)** - Payload creation framework focused on EDR bypass through DLL side-loading, ETW/AMSI patching, and syscall-based shellcode execution.
- 🐍 **[Inceptor](https://github.com/klezVirus/inceptor)** - Template-driven framework for AV and EDR evasion that transforms shellcode into various executable formats with multiple injection techniques.
- 🐹 **[OffensiveNim](https://github.com/byt3bl33d3r/OffensiveNim)** - Red teaming framework in Nim providing low-level primitives for shellcode loading, API unhooking, direct syscalls, reflective binary loading, and .NET assembly execution via CLR hosting.
- 🔐 **[Python-Crypter](https://github.com/wsummerhill/Python-Crypter)** - Shellcode encryptor and obfuscator supporting XOR and AES encryption with output formats including Base64, C hex, CSharp hex, manifest files, and chunked shellcode.
- 🔄 **[Simple Shellcode Crypter](https://github.com/Hue-Jhan/Simple-shellcode-crypter)** - C/C++ crypter applying three layers of obfuscation (custom Base64, XOR, and hexadecimal encoding) to shellcode for signature evasion.
- 🐚 **[Shhhloader](https://github.com/icyguider/Shhhloader)** - Shellcode loader that takes raw input and compiles a C++ stub implementing multiple AV/EDR bypass techniques, built via Python with Mingw-w64.
- 🎭 **[GadgetToJScript](https://github.com/med0x2e/GadgetToJScript)** - Generates .NET serialized gadgets that trigger assembly load/execution when deserialized via BinaryFormatter from JS, VBS, or VBA scripts.
- 🐘 **[DarkArmour](https://github.com/bats3c/darkarmour)** - Windows antivirus evasion tool that stores and executes encrypted binaries from memory without any bit touching disk.
- 🦀 **[HellBunny](https://github.com/Vasco0x4/ShellLoader_Hub)** - Malleable shellcode loader written in C and Assembly using direct or indirect syscalls to evade EDR hooks.

---

## Labs & Practice Environments

- 🧪 **[GOAD (Game of Active Directory)](https://github.com/Orange-Cyberdefense/GOAD)** - Ansible-automated Active Directory lab that deploys multi-domain forest architectures with intentionally misconfigured vulnerabilities, supporting local virtualization and cloud deployment as the de facto standard for AD red team training.
- 🎯 **[DreadGOAD](https://github.com/sliverarmory/DreadGOAD)** - Enhanced GOAD fork featuring 50+ real-world vulnerability scenarios, AWS auto-deployment, and variant generators, purpose-built for red/blue team assessments and AI attack-defense benchmarking.
- 🕸️ **[OWASP Juice Shop](https://owasp.org/www-project-juice-shop/)** - Modern JavaScript single-page application covering all OWASP Top 10 vulnerability categories, with a built-in scoreboard and progressive hint system, making it the ideal starting point for web application security practice.
- 🛡️ **[PortSwigger Web Security Academy](https://portswigger.net/web-security)** - Free browser-based lab platform from the Burp Suite team, offering structured learning paths and high-quality written tutorials covering SQL injection, XSS, SSRF, and other core web vulnerabilities.
- 💥 **[DVWA (Damn Vulnerable Web Application)](https://github.com/digininja/DVWA)** - Classic PHP/MySQL teaching application with adjustable difficulty levels, covering SQL injection, XSS, file inclusion, and other traditional web vulnerability categories, requiring local deployment.
- ☁️ **[CloudGoat](https://github.com/RhinoSecurityLabs/cloudgoat)** - AWS vulnerable scenario deployment tool maintained by Rhino Security Labs, using Terraform to rapidly build practice environments containing IAM misconfigurations, S3 permission issues, and other typical cloud security flaws.
- 🔐 **[Kubernetes Goat](https://github.com/madhuakula/kubernetes-goat)** - Intentionally vulnerable Kubernetes cluster environment for practicing container escape, RBAC abuse, network policy bypass, and other cloud-native attack techniques.
- 🏗️ **[TerraGoat](https://github.com/bridgecrewio/terragoat)** - Bridgecrew's intentionally insecure Terraform infrastructure codebase covering multi-cloud (AWS, Azure, GCP) IaC security misconfigurations, suitable for practicing cloud infrastructure auditing and attack surface discovery.
- 🎮 **[Hack The Box](https://www.hackthebox.com/)** - Gamified penetration testing platform offering machines and challenges spanning web, network, AD, and cloud scenarios, including dedicated Active Directory learning paths and the multi-cloud BlackSky series labs.
- 🧩 **[TryHackMe](https://tryhackme.com/)** - Guided cybersecurity learning platform providing structured AD attack/defense paths and room-based instruction, suitable for progressive learning from foundational concepts to practical attacks.

---

## Miscellaneous

- 🐉 **[Kali Linux](https://www.kali.org/)** - The industry-standard penetration testing and security auditing OS, maintained by Offensive Security, preloaded with 600+ tools including Metasploit, Nmap, and Burp Suite, and officially supported for OSCP certification.
- 🦜 **[Parrot Security OS](https://www.parrotsec.org/)** - Lightweight, privacy-focused security distribution with 800+ tools, built-in AnonSurf for system-wide Tor routing, and a hardened kernel, suitable for low-spec hardware and anonymity-sensitive operations.
- 🏴 **[BlackArch Linux](https://blackarch.org/)** - Arch Linux-based distribution featuring 2,800+ specialized security tools, designed for advanced researchers who want to build a bespoke toolchain from the ground up.
- 🧑‍💻 **[BackBox](https://www.backbox.org/)** - Ubuntu-based Linux distribution for penetration testing and security assessment, offering stability with meta-packages for web, wireless, and reverse-engineering testing.
- 👻 **[Tails](https://tails.net/)** - The Amnesic Incognito Live System that forces all internet connections through Tor and leaves no trace on the host computer, designed for anonymity, censorship circumvention, and high-risk operational security.
- 🦠 **[REMnux](https://remnux.org/)** - Linux toolkit specifically designed for reverse-engineering and analyzing malicious software, providing a curated environment for malware analysis and forensic investigation.
- 🕵️ **[Whonix](https://www.whonix.org/)** - Anonymous OS based on Tor with a unique architecture that isolates the user's activities from the network, preventing IP leaks and protecting against attacks that target the operating system.
- 🛡️ **[Kali NetHunter](https://www.kali.org/get-kali/#kali-mobile)** - Mobile penetration testing platform for Android devices, bringing Kali tools and wireless attack capabilities to smartphones and tablets for on-the-go assessments.
- 🔧 **[Cervantes](https://github.com/CervantesSec/cervantes)** - Open-source collaborative platform for pentesters and red teams, streamlining project organization, client management, vulnerability tracking, and reporting in a centralized location.
- 📊 **[Dradis](https://dradis.com/)** - Self-hosted collaboration and reporting platform for pentesters with 47+ scanner integrations (Burp, Nessus, OpenVAS), an Issue Library with Rules Engine for consistent findings, and on-premises AI-assisted reporting via Ollama.
- 🎯 **[PlexTrac](https://plextrac.com/)** - Purpose-built red team and purple team engagement platform with Runbooks for TTP-level operator coordination, MITRE ATT&CK-mapped execution tracking, and AI-assisted reporting features.
- 📋 **[DefectDojo](https://defectdojo.com/)** - Open-source vulnerability management platform that treats pentests as first-class data, with Engagement containers for structured findings, deduplication across 500+ security tools, and remediation tracking through Jira/GitHub integration.
- 🧪 **[Viper](https://github.com/FunnyWolf/Viper)** - Free adversary simulation and red teaming platform with a visual UI, 100+ post-exploitation modules covering MITRE ATT&CK phases, pivot graph, built-in defense evasion, Python custom modules, and an integrated LLM agent for intelligent decision support.
- 🗺️ **[Red Team Infrastructure Wiki](https://github.com/bluscreenofjeff/Red-Team-Infrastructure-Wiki)** - Comprehensive community wiki collecting resources for red team infrastructure hardening, C2 traffic modification (Malleable C2, Empire profiles), domain fronting, and third-party C2 channels.
- 🏗️ **[Red Team Infrastructure Wiki (gyorijanos)](https://github.com/gyorijanos/Red-Team-Infrastructure-Wiki)** - Additional wiki resource for red team infrastructure setup, covering Apache mod_rewrite automation, Cobalt Strike profile configuration, and operational security considerations.
- 💻 **[Dell Precision 7680](https://www.dell.com/en-us/work/shop/dell-laptops-and-notebooks/precision-7680-mobile-workstation/spd/precision-16-7680-laptop)** - Mobile workstation for red team operators with NVIDIA RTX 5000 Blackwell GPU, up to 192GB RAM, 16TB storage across 4 M.2 slots, and Cryo-Tech cooling for sustained Hashcat cracking and large-scale AD forest simulation.
- 💻 **[Lenovo ThinkPad P16s Gen 3](https://www.lenovo.com/us/en/p/laptops/thinkpad/thinkpadp/thinkpad-p16s-gen-3/len101t0087)** - MIL-STD-810H ruggedized workstation with vapor chamber cooling, up to 128GB RAM, 4 M.2 slots supporting 8TB, and the reliability of ThinkPad keyboards for enterprise red team deployments.
- 💻 **[HP ZBook Fury 16 G11](https://www.hp.com/us-en/workstations/zbook-fury.html)** - Mobile workstation with 128GB RAM, 4 SSD slots, optional 6000-nit mini-LED display, and ZCool three-fan system for teams handling terabyte-scale memory dumps and forensics workloads.
- 🔌 **[WiFi Pineapple Mark VII](https://shop.hak5.org/products/wifi-pineapple)** - Wireless attack platform for rogue access point emulation, credential harvesting during wireless audits, and man-in-the-middle operations, a staple in physical red team engagements.
- 🦆 **[USB Rubber Ducky](https://shop.hak5.org/products/usb-rubber-ducky)** - Keystroke injection tool disguised as a USB flash drive that executes pre-programmed payloads at machine speed, used for physical access initial access and rapid payload delivery.
- 📡 **[HackRF One](https://greatscottgadgets.com/hackrf/)** - Software Defined Radio (SDR) platform covering 1 MHz to 6 GHz, enabling analysis and replay of IoT wireless protocols, RF reconnaissance, and custom protocol development for red team hardware assessments.
- 📶 **[Alfa AWUS036ACHM](https://www.alfa.com.tw/products/awus036achm)** - Long-range dual-band wireless adapter with monitor mode and packet injection support, essential for wireless penetration testing and RF assessment with proper driver compatibility.
- 🎯 **[GoFetch](https://github.com/GoFetchAD/GoFetch)** - BloodHound attack path automation tool that automatically exercises attack plans, streamlining the execution of privilege escalation routes discovered through AD graph analysis.
- ⚡ **[ANGRYPUPPY](https://github.com/vysec/ANGRYPUPPY)** - BloodHound attack path automation for Cobalt Strike, enabling rapid execution of discovered AD escalation paths directly from the C2 framework.
- 💀 **[DeathStar](https://github.com/byt3bl33d3r/DeathStar)** - Python script that uses Empire's RESTful API to automate gaining Domain Admin rights in Active Directory environments, orchestrating multiple attack techniques.
- 🧠 **[SharpHound](https://github.com/BloodHoundAD/SharpHound)** - C# rewrite of the BloodHound ingestor for Windows environments, providing optimized AD data collection for attack path analysis.
- 🐍 **[BloodHound.py](https://github.com/fox-it/BloodHound.py)** - Python-based BloodHound ingestor built on Impacket, enabling AD enumeration from Linux/macOS without requiring Windows tooling.
- 🔑 **[SessionGopher](https://github.com/fireeye/SessionGopher)** - PowerShell tool that uses WMI to extract saved session information for WinSCP, PuTTY, FileZilla, and Microsoft Remote Desktop, recovering credentials from remote access tool configs.
- 🦞 **[LaZagne](https://github.com/AlessandroZ/LaZagne)** - Open-source credential recovery tool that retrieves passwords stored locally by applications including browsers, email clients, databases, and WiFi configurations.
- 🐧 **[mimipenguin](https://github.com/huntergregal/mimipenguin)** - Linux credential dumper that extracts login passwords from the current desktop user by reading process memory, adapted from the Mimikatz concept.
- 🗝️ **[KeeThief](https://github.com/HarmJ0y/KeeThief)** - Tool for extracting KeePass 2.X key material from memory, backdooring the KeePass trigger system, and enumerating KeePass configurations during red team operations.
- ⚡ **[PSAttack](https://github.com/jaredhaight/PSAttack)** - Self-contained custom PowerShell console combining the best offensive PowerShell projects for rapid deployment in constrained environments.
- 🔓 **[Internal Monologue](https://github.com/eladshamir/Internal-Monologue)** - Technique for retrieving NTLM hashes without touching LSASS memory, evading credential dumping detection by abusing the authentication protocol stack.
- 🧊 **[icebreaker](https://github.com/DanMcInerney/icebreaker)** - Tool for obtaining plaintext Active Directory credentials from internal networks where the attacker is outside the AD environment, leveraging network protocol weaknesses.
- 🗂️ **[PowerUpSQL](https://github.com/NetSPI/PowerUpSQL)** - PowerShell toolkit for attacking SQL Server instances, covering discovery, privilege escalation, and command execution in database-focused red team operations.
- 📬 **[MailSniper](https://github.com/dafthack/MailSniper)** - PowerShell tool for searching Exchange and Office 365 mailboxes for sensitive terms including passwords, insider intel, and network architecture details.
- 🪟 **[WMIOps](https://github.com/ChrisTruncer/WMIOps)** - PowerShell script using WMI to perform remote actions on Windows hosts, designed for penetration testing and red team lateral movement and execution.
- 🎣 **[Inveigh](https://github.com/Kevin-Robertson/Inveigh)** - Windows PowerShell LLMNR/mDNS/NBNS spoofer and man-in-the-middle tool for capturing NetNTLM hashes and enabling relay attacks in Windows environments.
- 🔬 **[Dome](https://github.com/v4d1/Dome)** - Fast Python subdomain enumeration tool performing active and passive scanning, with integrated open port search for efficient reconnaissance workflows.
- 🛠️ **[RedTeam_toolkit](https://github.com/signorrayan/RedTeam_toolkit)** - Open-source Django offensive web application consolidating useful red teaming tools into a centralized platform for streamlined operations.
- 💉 **[ImpulsiveDLLHijack](https://github.com/knight0x07/ImpulsiveDLLHijack)** - C# tool automating the discovery and exploitation of DLL hijacking vulnerabilities in target binaries, weaponizing discovered paths for EDR evasion during red team operations.
- 🎯 **[PowerShellArmoury](https://github.com/cfalta/PowerShellArmoury)** - Curated collection of PowerShell offensive tools and scripts packaged for security professionals and red teamers.
- 🌌 **[Nebula](https://github.com/berylliumsec/nebula)** - AI-powered ethical hacking assistant providing intelligent guidance and automation for offensive security workflows.
- 🔓 **[KRBUACBypass](https://github.com/wh0amitz/KRBUACBypass)** - UAC bypass technique by abusing Kerberos tickets, enabling privilege elevation without triggering standard UAC prompts.
- 🌳 **[eviltree](https://github.com/t3l3machus/eviltree)** - Python3 remake of the classic tree command with keyword/regex search capabilities, highlighting matching files during reconnaissance.
- 💾 **[NativeDump](https://github.com/ricardojoserf/NativeDump)** - Tool for dumping LSASS memory using only native APIs by hand, avoiding common detection signatures associated with credential dumping tools.
- 📁 **[PipeViewer](https://github.com/cyberark/PipeViewer)** - Tool that displays detailed information about named pipes in Windows, useful for understanding IPC attack surfaces during red team reconnaissance.
- 📱 **[apk2url](https://github.com/n0mi1k/apk2url)** - OSINT tool for quickly extracting IP addresses and URL endpoints from APK files through disassembly and decompilation, useful for mobile reconnaissance.
- 🕸️ **[Pyramid](https://github.com/naksyn/Pyramid)** - Tool designed to help operators work within EDR blind spots, providing evasion capabilities for post-exploitation activities.
- ⚡ **[skanuvaty](https://github.com/Esc4iCEscEsc/skanuvaty)** - Dangerously fast DNS/network/port scanner written in Rust, designed for rapid reconnaissance across large target ranges.
- 🎯 **[Offensive-OSINT-Tools](https://github.com/wddadk/Offensive-OSINT-Tools)** - Curated collection of open-source intelligence tools for pentesting and red teaming, covering reconnaissance and information gathering workflows.
- 🔍 **[shortscan](https://github.com/bitquark/shortscan)** - IIS short filename enumeration tool for discovering hidden files and directories on Microsoft IIS web servers.
- 🧰 **[Red Team Attack Lab](https://github.com/marcosrivasr/Red-Team-Attack-Lab)** - TTP testing and research lab environment for validating attack techniques and building detection engineering scenarios.
- ☁️ **[RedCloudOS](https://github.com/RedCloudOS/RedCloudOS)** - Cloud adversary simulation operating system for red teams to assess the security posture of leading cloud service providers.
- 🔴 **[RedEye](https://github.com/cisagov/RedEye)** - Tool for managing and visualizing red team data during operations, including attack path tracking and evidence organization.
- 📝 **[PeTeReport](https://github.com/1modm/petereport)** - Open-source application vulnerability reporting tool for structured pentest documentation and client deliverables.

Exploiting BlueKeep (CVE-2019-0708) on Windows 7
## Objective
Gain remote access to an unpatched Windows 7 system via the BlueKeep RDP vulnerability
using Metasploit.
## Lab Setup
- Attacker: Kali Linux
- Target: Windows 7 (Unpatched, RDP Enabled)
- Network: NAT / Host-Only

## Tools Used
- Metasploit Framework
- Kali Linux
- Windows 7

## Exploitation Process
### Phase 1: Recon & Setup
- Launch Metasploit
- Search BlueKeep module
- Configure RHOSTS and RDP settings

### Phase 2: Payloads Used
#### 1. Reverse Shell
- Payload: windows/x64/shell_reverse_tcp
- Result: Command shell access
#### 2. VNC Injection
- Payload: windows/x64/vncinject/reverse_tcp
- Result: GUI access to victim desktop
#### 3. Meterpreter
- Payload: windows/x64/meterpreter/reverse_tcp
- Result: Advanced control (keylogging, screenshots, etc.)
## Screenshots
See `/screenshots` folder
## Commands Used
See `/commands/commands-used.txt`
## Ethical Disclaimer
This project was conducted in a controlled lab environment for educational purposes only.
Unauthorised ecploitation of systems is illegal
## Author
Nweke Chigozie

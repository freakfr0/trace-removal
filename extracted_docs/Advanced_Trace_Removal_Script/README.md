# Advanced Trace Removal Script

This script is designed to securely remove traces of activity from a server, which may be used for cleaning up logs, history, processes, and other sensitive information. It is important to note that this script is intended for educational and ethical hacking purposes only. Misuse of this script can be illegal and unethical.

## Features
The script performs the following tasks:

1. **Check for Root Privileges**: Ensures the script is run with root privileges.
2. **Delete Advanced Logs**: Removes log files from directories such as `/var/log`, `/tmp`, and `/root/.bash_history` using secure deletion methods.
3. **Clear Command and Process History**: Clears the shell history and any process traces for commands like `bash`, `python`, and others.
4. **Hide Suspicious Processes**: Kills processes that might indicate unauthorized activities or suspicious commands (e.g., `nc`, `wget`, `curl`).
5. **Modify Timestamps**: Alters file timestamps to a fixed date to remove traces of file activities.
6. **Clean Firewall Settings**: Resets the firewall settings and disables the firewall.
7. **Remove Suspicious Users**: Removes potentially malicious users (e.g., `test`, `admin`, `hacker`).
8. **Remove SSH Keys and Credentials**: Deletes SSH keys and credentials that might provide unauthorized access.
9. **Delete Sensitive System Files**: Removes sensitive files like configuration, logs, and system credentials (e.g., `passwd`, `shadow`).
10. **Clean Network Settings**: Resets network settings, flushing IP addresses and routes.
11. **Hide the Script**: Finally, the script deletes itself to remove any trace of its execution.

## Usage

1. **Make the Script Executable**: Before running the script, you need to make it executable. Use the following command:

    ```bash
    chmod +x cleanup.sh
    ```

2. **Run the Script as Root**: Execute the script with root privileges to allow it to perform system-level changes.

    ```bash
    sudo ./cleanup.sh
    ```

## Important Notes

- **Educational Use Only**: This script is intended for educational purposes in controlled environments like penetration testing labs or CTF challenges.
- **Legal Implications**: Unauthorized use of this script in real-world environments can be considered malicious and illegal. Always ensure you have explicit permission before running this script.

## License
This script is released under the MIT License for educational purposes.



Explanation

    Script: Translated the original script from Arabic to English. It performs various tasks to erase traces of system activity like logs, processes, SSH keys, and more. It should only be run in ethical environments where permission has been granted.
    README.md: Describes the purpose, features, usage, and important legal considerations for using the script.

Make sure to use the script responsibly, ensuring you are in a legal and ethical environment before executing it.

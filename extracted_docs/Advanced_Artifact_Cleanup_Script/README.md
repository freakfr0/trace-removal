# Advanced Artifact Cleanup Script

This script is designed to perform advanced cleanup and stealth measures on a Linux server. It erases system logs, modifies timestamps, hides processes, resets network configurations, deletes sensitive files, and more. It is intended to be used for privacy or security purposes on your personal systems.

### Features:
- **Delete logs**: Removes system logs and histories.
- **Modify timestamps**: Alters the timestamps of all files to prevent traceability.
- **Hide processes**: Uses techniques like `chroot` and `LD_PRELOAD` to hide suspicious processes.
- **Reset network settings**: Resets firewall and network settings to avoid detection.
- **Delete suspicious users**: Removes specific suspicious users from the system.
- **Delete SSH keys and authentication files**: Removes sensitive SSH keys.
- **Delete sensitive system files**: Deletes crucial files like `/etc/passwd`, `/etc/shadow`, and others.
- **Self-destruct**: Hides and deletes the script itself to erase traces.
- **Use Proxy**: Routes traffic through a proxy to hide the origin of connections.
- **Obfuscate IP address**: Changes the system's IP address to avoid detection.
- **Memory tampering**: Disables memory dump to avoid sensitive data leaks.

### Prerequisites:
- The script must be executed with root privileges.
- The following tools are required:
  - `shred`
  - `proxychains4`
  - `steghide`

### How to Run:
1. **Download the script** to your server.
2. **Make the script executable**:
   ```bash
   chmod +x cleanup_script.sh

Run the script as root:

    sudo ./cleanup_script.sh

Warning:

    This script is powerful and will remove critical system logs and files. It should only be used on machines you control, and it is highly recommended to back up important data before running it.

License:

This script is provided for educational and personal use only. Use it responsibly and in compliance with all applicable laws.





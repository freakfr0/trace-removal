# Advanced Cleanup Script

This script is designed to perform various actions that may erase traces from a system to cover up suspicious activity. It is primarily intended for educational purposes to learn about system administration and security.

**Note:** This script should only be run in a controlled environment, such as a Virtual Machine or testing environment, to avoid legal or ethical issues.

## Features

- **Check for root privileges:** Ensures that the script is run with root access.
- **Delete logs:** Deletes log files from various directories to remove traces.
- **Modify file timestamps:** Alters the timestamps of files to hide traces of access.
- **Hide suspicious processes:** Hides running suspicious processes and uses `chroot` to hide them.
- **Reset network settings and firewall:** Clears firewall rules and disables network logs.
- **Delete suspicious users:** Deletes system users that are likely to be backdoor accounts.
- **Delete SSH keys:** Clears SSH keys to remove authentication records.
- **Delete sensitive system files:** Erases sensitive files that may contain system and user information.
- **Hide the script itself:** Embeds the script inside an image using `steghide` to make it harder to find.
- **Use Proxy:** Hides your identity by using a proxy through `proxychains`.

## Usage

1. **Run the script as root:**

    ```bash
    sudo bash cleanup_script.sh
    ```

2. The script will automatically execute the steps mentioned above to clean up the system.

3. **Note:** The script will delete data permanently and cannot be undone. Please use caution.

## Requirements

- `shred` command (comes pre-installed on most Linux distributions)
- `steghide` for hiding the script inside an image
- `proxychains4` for proxy use

## Disclaimer

This script is for **educational purposes only**. Misuse of this script for illegal activities is not supported. Always ensure you have permission to run scripts like this on any system.

This README outlines the script's purpose, features, usage, and disclaimer. The script performs actions that can be destructive, so it should only be used responsibly.


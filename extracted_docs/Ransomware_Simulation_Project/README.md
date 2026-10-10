# Ransomware Simulation Project

This project simulates a ransomware attack, encrypting files using AES and RSA encryption, and displays a ransom message to the user. It also includes techniques for hiding network traffic and installing rootkits for persistent access. The simulation uses tools like Metasploit for exploitation and Python for encryption.

## Features
- **RSA & AES Encryption**: Encrypts files using AES encryption and encrypts the AES key with RSA.
- **Zero-Day Exploit**: Exploits the EternalBlue vulnerability (MS17-010).
- **Traffic Camouflage**: Hides network traffic using NAT.
- **Rootkit Installation**: Installs a rootkit for maintaining persistent access.
- **Ransom Message**: Displays a ransom message demanding Bitcoin for file decryption.
- **Encrypted Key Storage**: Stores the AES encryption key in an encrypted form.

## Installation
1. Install required Python libraries:
   ```bash
   pip install pycryptodome requests


    Ensure Metasploit is installed and configured properly for the exploit functionality to work.

    Adjust the target folder for the simulation:
        Modify the target_folder variable in the script to point to the folder you want to simulate the attack on.

Usage

    Run the Python script:

    python ransomware_simulation.py

    The script will simulate the ransomware attack, encrypt files in the specified folder, display the ransom message, and send ransom details to a fake server.

Important Notes

    Ethical Usage: This project is for educational and ethical hacking purposes only. Do not use it for malicious purposes.
    Legal Disclaimer: The use of exploits and hacking techniques in unauthorized environments is illegal. This project is intended for use in controlled, ethical environments.

License

This project is licensed under the MIT License.


Let me know if you need further modifications or explanations!


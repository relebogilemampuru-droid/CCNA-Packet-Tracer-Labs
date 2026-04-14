# 🔒 Lab: Securing Remote Access with SSH

### Objective
To replace insecure Telnet access with encrypted SSH (Secure Shell) to ensure management traffic remains confidential.

### Key Configurations:
* **Hostname & Domain Name:** Set unique identifiers for RSA key generation.
* **RSA Key Generation:** Configured `crypto key generate rsa` with a 1024-bit modulus.
* **User Authentication:** Created local usernames with secret passwords.
* **VTY Line Hardening:** Restricted transport input to SSH only (`transport input ssh`).

### Verification Commands:
* `show ip ssh` - To verify version and authentication timeout.
* `show ssh` - To view active encrypted sessions.

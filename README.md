CyberShield 🔐
A Python-based cybersecurity toolkit built to demonstrate real-world security principles including encryption, access control, multi-factor authentication, and audit logging.

Built as part of a Global Professional Internship (GPI) with Cloud Counselage Pvt. Ltd. in the Cyber Security domain.


Features

AES-256-CBC Encryption — Symmetric encryption for securing sensitive data at rest
RSA-2048 Key Exchange — Asymmetric encryption for secure key transmission
Role-Based Access Control (RBAC) — Granular permission management by user roles
Multi-Factor Authentication (MFA) — Extra verification layer beyond passwords
Audit Logging — Tamper-evident logs of all system access and actions
PII Detection — Identifies and flags personally identifiable information in data


Tech Stack
ComponentTechnologyLanguagePython 3.xSymmetric EncryptionAES-256-CBC (via cryptography library)Asymmetric EncryptionRSA-2048Access ControlCustom RBAC implementationAuthenticationMFA with TOTPLoggingPython logging module with structured output

Project Structure
CyberShield/
├── encryption/
│   ├── aes_encryption.py       # AES-256-CBC encrypt/decrypt
│   └── rsa_key_exchange.py     # RSA-2048 key generation & exchange
├── access_control/
│   ├── rbac.py                 # Role and permission management
│   └── mfa.py                  # Multi-factor authentication
├── audit/
│   └── audit_logger.py         # Audit trail logging
├── pii/
│   └── pii_detector.py         # PII scanning and flagging
├── main.py                     # Entry point
└── requirements.txt

Getting Started
Prerequisites

Python 3.8 or higher
pip

Installation
bash# Clone the repository
git clone https://github.com/your-username/CyberShield.git
cd CyberShield

# Install dependencies
pip install -r requirements.txt
Run the project
bashpython main.py

How It Works
Encryption flow
Data is encrypted using AES-256-CBC, where the AES key itself is secured using RSA-2048 public key encryption. This hybrid approach combines the speed of symmetric encryption with the security of asymmetric key exchange.
Access control
Users are assigned roles (e.g. admin, analyst, viewer). Each role has a defined set of permissions. Access to any resource is checked against the user's role before being granted.
Audit logging
Every login attempt, data access, and permission change is written to a structured audit log with timestamps, user IDs, and action types — making the system traceable and accountable.

Security Concepts Demonstrated

Hybrid encryption (AES + RSA)
Principle of least privilege (RBAC)
Defence in depth (MFA + access control + logging)
Data privacy (PII detection)
Non-repudiation (audit trails)


What I Learned
This project gave me hands-on experience implementing security concepts that are typically only seen in enterprise systems. Key takeaways:

How AES-CBC mode works and why IV (Initialization Vector) matters
The difference between encryption at rest vs in transit
How RBAC reduces attack surface compared to flat permission models
Why audit logs are critical for incident response


Documentation
This project was delivered with full project management documentation:

Project Charter
Software Requirements Specification (SRS)
RAID Log
Work Breakdown Structure (WBS)
Project Schedule
Lessons Learnt Log


Author
Bhumaa
BCA Student | Cybersecurity & Cloud Computing
Global Professional Intern @ Cloud Counselage Pvt. Ltd.
LinkedIn · GitHub

License
This project is for educational purposes. Feel free to explore the code and concepts.

# 🔐 SSH (Secure Shell) Notes

## 📌 What is SSH?

**SSH (Secure Shell)** is a network protocol used to securely connect and communicate with remote systems over an unsecured network. It provides encrypted communication, authentication, and secure remote administration.

- **Full Form:** Secure Shell
- **Layer:** Application Layer
- **Default Port:** 22
- **Protocol Type:** Secure Remote Access Protocol
- **Transport Protocol:** TCP

---

## 🎯 Why SSH is Used

- Secure remote server login
- Remote command execution
- Secure file transfer
- Server administration
- Git and GitHub authentication
- Secure tunneling and port forwarding

---


## 🔄 How SSH Works

```text
Client (Your Computer)
        │
        │  SSH Request
        ▼
Authentication (Password or SSH Key)
        │
        │  Encrypted Communication
        ▼
Remote Server
```

---

## 🔑 SSH Authentication Methods

### 1. Password Authentication
- User enters username and password.
- Server verifies credentials.
- Secure connection is established.

### 2. Public Key Authentication (Recommended)
- User generates an SSH key pair.
- Public key is stored on the server.
- Private key remains on the local machine.
- Server verifies the key and grants access.

---

## 🔐 SSH Key Pair

```text
SSH Key Pair
│
├── Public Key  → Shared with Server/GitHub
└── Private Key → Kept Secret on Your Computer
```

---




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

## 📂 Common SSH Commands

### Generate SSH Key

```bash
ssh-keygen -t ed25519 -C "your-email@example.com"
```

### Start SSH Agent

```bash
eval "$(ssh-agent -s)"
```

### Add Key to SSH Agent

```bash
ssh-add ~/.ssh/id_ed25519
```

### Display Public Key

```bash
cat ~/.ssh/id_ed25519.pub
```

### Connect to Remote Server

```bash
ssh username@server-ip
```

### Test GitHub Connection

```bash
ssh -T git@github.com
```

---

## 🔄 SSH Working Flow

```text
1. Client initiates SSH connection
            │
            ▼
2. Server sends public key information
            │
            ▼
3. Client verifies server identity
            │
            ▼
4. Authentication (Password or SSH Key)
            │
            ▼
5. Session keys are generated
            │
            ▼
6. Secure encrypted communication starts
```

---


## 🌐 SSH in GitHub

SSH allows you to interact with GitHub repositories securely without entering your username and password every time.

### Clone Repository

```bash
git clone git@github.com:username/repository.git
```

### Push Changes

```bash
git push origin main
```

### Pull Changes

```bash
git pull origin main
```

---

## ⚡ Advantages of SSH

- Encrypted communication
- Strong authentication mechanism
- Secure remote administration
- Supports automation and scripting
- More secure than Telnet
- Widely used with Git and GitHub

---



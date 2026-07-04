# Computer Networking

  Computer Networking means Number of computer are placed at different location connected through the network so they can share/transport the resources through that network is called computer networking 
  
OR

Computer Networking is the process of connecting two or more computers or devices so they can communicate and share data, resources, and services with each other.


## Diagram

![Computer Networking](images/CN_example.png)

# 🌐 OSI (Open Systems Interconnection) Model

## 📖 Introduction

The **OSI (Open Systems Interconnection) Model** is a conceptual framework developed by the International Organization for Standardization (ISO) to standardize communication between different computer systems.

It divides the communication process into **7 different layers**, where each layer performs a specific task.

The main purpose of the OSI model is to ensure that hardware and software from different vendors can communicate with each other.

Although the Internet mainly follows the TCP/IP model, the OSI model is widely used for learning networking concepts and troubleshooting network issues.


## 🎯 Why Do We Need the OSI Model?

Before the OSI model, every company developed its own networking protocols, making communication between different devices difficult.

The OSI model solves this problem by:

- Standardizing communication
- Reducing complexity
- Improving interoperability
- Simplifying troubleshooting
- Allowing independent development of each layer


## 🖼️ OSI Model Diagram

![OSI Model](images/OSI_model.png)

## 🔄 Data Flow

```mermaid
flowchart TD
A[Application]
B[Presentation]
C[Session]
D[Transport]
E[Network]
F[Data Link]
G[Physical]

A --> B --> C --> D --> E --> F --> G
```

# 📚 Seven Layers of the OSI Model

## 7️⃣ Application Layer

### Purpose

Application layer provides network services directly to end users and applications.

### Responsibilities

- Email
- Web browsing
- File transfer
- Remote login

### Protocols used in Application Layer

- HTTP
- HTTPS
- FTP
- SMTP
- DNS

### Devices

- Computer
- Mobile
- Browser

### Real-Life Example

When you open YouTube in your browser, the request starts from the Application Layer.

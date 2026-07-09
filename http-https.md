# 🌐 HTTP & HTTPS 

## What is HTTP?

**HTTP (HyperText Transfer Protocol)** is an application layer protocol used for communication between a web browser (client) and a web server. It allows users to request and receive web pages, images, videos, and other resources over the internet.

- **Full Form:** HyperText Transfer Protocol
- **Layer:** Application Layer (TCP/IP Model)
- **Default Port:** 80
- **Protocol Type:** Stateless
- **Transport Protocol:** TCP

---

## 🔄 How HTTP Works

```text
Browser (Client)
       │
       │  HTTP Request
       ▼
Web Server
       │
       │  HTTP Response
       ▼
Browser Displays Web Page
```

### Step-by-Step Process

1. User enters a URL in the browser.
2. Browser sends an **HTTP Request** to the server.
3. Server processes the request.
4. Server sends an **HTTP Response**.
5. Browser displays the requested content.

---

## 📨 HTTP Request Methods

| Method | Description |
|--------|-------------|
| GET | Retrieves data from the server |
| POST | Sends data to the server |
| PUT | Updates existing data |
| DELETE | Removes data from the server |
| PATCH | Partially updates data |

---


## ❌ Limitations of HTTP

- Data is transmitted in **plain text**.
- No encryption or confidentiality.
- Vulnerable to:
  - Eavesdropping
  - Man-in-the-Middle (MITM) attacks
  - Data modification
  - Session hijacking

---

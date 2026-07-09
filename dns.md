# Domain Name Systeam (DNS)

## What is DNS?
**Domain Name System (DNS)** is a distributed naming system that translates **human-readable domain names** into **IP addresses**.

**Example:**
```text
www.google.com  →  142.250.182.14
```

> DNS is known as the **Phonebook of the Internet** because it converts domain names into IP addresses.

---

## 🎯 Why DNS is Important
- Easy to remember domain names instead of IP addresses.
- Helps browsers locate websites quickly.
- Supports web browsing, email, and other internet services.
- Provides scalability and efficient internet communication.

---

## ⚙️ How DNS Works

```text
User enters www.google.com
          │
          ▼
Browser Cache
          │
          ▼
DNS Resolver
          │
          ▼
Root Server (.)
          │
          ▼
TLD Server (.com)
          │
          ▼
Authoritative DNS Server
          │
          ▼
Returns IP Address
          │
          ▼
Browser loads the website
```

---

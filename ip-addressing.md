# IP Addressing

## Definetion :

**IP (Internet Protocol) Addressing** is a method used to uniquely identify devices on a network. It enables communication between devices by providing a logical address for sending and receiving data packets across local and global networks.

---

## Why IP Addressing is Important

- Uniquely identifies each device on a network.
- Enables communication between devices.
- Assists routers in forwarding data to the correct destination.
- Supports communication over both local networks (LAN) and the Internet.

---

# Types of IP Addresses

#### There are two types of IP (Internet protocol)
- IPv4 (Internet Protocol version 4)
- IPv6 (Internet Protocol version 6)

### IPv4 (Internet Protocol Version 4)

- Uses a **32-bit** address.
- Represented in **dotted-decimal notation**.
- Consists of **4 octets**, each ranging from **0 to 255**.
- Most widely used IP addressing scheme.

**Example:**

```text
192.168.1.10
```

---

### IPv6 (Internet Protocol Version 6)

- Uses a **128-bit** address.
- Represented in **hexadecimal notation**.
- Developed to overcome IPv4 address exhaustion.
- Supports a significantly larger address space.

**Example:**

```text
2001:db8:85a3::8a2e:370:7334
```

---

## IPv4 Address Structure

An IPv4 address is divided into four 8-bit sections (octets).

```text
192      .168      .1      .10
└──8 bits┘└──8 bits┘└8 bits┘└8 bits┘

Total = 32 bits
```

---


## Components of an IP Address

Every IPv4 address consists of two logical parts:

```text
+----------------+----------------+
|   Network ID   |    Host ID     |
+----------------+----------------+
```

- **Network ID:** Identifies the network to which the device belongs.
- **Host ID:** Identifies a specific device within that network.

---

## IP Address Classes

| Class | Address Range | Default Subnet Mask | Purpose |
|-------|---------------------------|-----------------|----------------|
| A | 1.0.0.0 – 126.255.255.255 | 255.0.0.0 (/8) | Large Networks |
| B | 128.0.0.0 – 191.255.255.255 | 255.255.0.0 (/16) | Medium Networks |
| C | 192.0.0.0 – 223.255.255.255 | 255.255.255.0 (/24) | Small Networks |
| D | 224.0.0.0 – 239.255.255.255 | N/A | Multicast |
| E | 240.0.0.0 – 255.255.255.255 | N/A | Experimental |

---

## Public vs Private IP Addresses

### Public IP Address
- Assigned by an Internet Service Provider (ISP).
- Accessible over the Internet.
- Used for communication between external networks.

### Private IP Address
- Used within local area networks (LANs).
- Not directly accessible from the Internet.
- Conserves public IP addresses.


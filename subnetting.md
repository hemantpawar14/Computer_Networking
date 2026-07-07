# Subnetting

## Definetion :

**Subnetting** is the process of dividing a large IP network into multiple smaller logical networks called **subnets**. It improves network performance, enhances security, and makes efficient use of IP addresses.

---

## Why Subnetting used?

- Reduces network congestion.
- Improves network performance.
- Enhances security by isolating networks.
- Efficient utilization of IP addresses.
- Simplifies network management.

---

## Key Terminologies

### Network Address
The **first IP address** of a subnet. It identifies the subnet and **cannot** be assigned to a host.

**Example:**
```text
192.168.1.0/24
```

---


### Host Address
The IP addresses that can be assigned to devices within a subnet.

**Example:**
```text
192.168.1.1 – 192.168.1.254
```

---

## Broadcast Address
The **last IP address** of a subnet. It is used to send data to **all devices** in that subnet.

**Example:**
```text
192.168.1.255
```

---

## Subnet Mask

A **Subnet Mask** separates the **Network ID** and **Host ID** of an IP address.

**Example:**

| CIDR | Subnet Mask |
|------|-------------|
| /24 | 255.255.255.0 |
| /25 | 255.255.255.128 |
| /26 | 255.255.255.192 |
| /27 | 255.255.255.224 |
| /28 | 255.255.255.240 |
| /29 | 255.255.255.248 |
| /30 | 255.255.255.252 |

---

## CIDR (Classless Inter-Domain Routing)

CIDR is a notation used to represent the subnet mask using a prefix length.

**Example:**

```text
192.168.1.0/24
```

Here, `/24` means the first **24 bits** represent the network portion.

---

## Subnetting Formula

### Number of Subnets

```text
2ⁿ
```

Where:

- **n** = Number of borrowed bits

---

### Number of Hosts per Subnet

```text
2ʰ − 2
```

Where:

- **h** = Number of host bits
- `-2` accounts for the **Network Address** and **Broadcast Address**.

---

## Example

Given the network:

```text
192.168.1.0/24
```

Divide it into **4 subnets**.

- Borrow **2 bits**
- New prefix: **/26**
- Subnet mask: **255.255.255.192**

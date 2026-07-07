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

  | Subnet | Host Range | Broadcast |
|---------|------------|-----------|
| 192.168.1.0/26 | 192.168.1.1 – 192.168.1.62 | 192.168.1.63 |
| 192.168.1.64/26 | 192.168.1.65 – 192.168.1.126 | 192.168.1.127 |
| 192.168.1.128/26 | 192.168.1.129 – 192.168.1.190 | 192.168.1.191 |
| 192.168.1.192/26 | 192.168.1.193 – 192.168.1.254 | 192.168.1.255 |

---

## FLSM vs VLSM

| FLSM | VLSM |
|------|------|
| Fixed subnet size | Variable subnet size |
| Same subnet mask for all subnets | Different subnet masks |
| Easier to configure | Better IP address utilization |
| May waste IP addresses | Minimizes IP address wastage |

---

## Quick Summary

- **Subnetting** divides a large network into smaller subnetworks.
- **Subnet Mask** separates the Network ID and Host ID.
- **CIDR** represents the subnet mask using prefix notation (e.g., `/24`).
- **Network Address** is the first IP of a subnet.
- **Broadcast Address** is the last IP of a subnet.
- **Host Addresses** are the usable IP addresses between the network and broadcast addresses.
- **Subnets Formula:** `2ⁿ`
- **Hosts Formula:** `2ʰ − 2`

---


# Network Address Translation (NAT)

## 📖 What is NAT?

Network Address Translation (NAT) is a process performed by a router to translate private IP addresses into public IP addresses (and vice versa). It allows multiple devices in a private network to access the Internet using a single public IP address.

---

## 🎯 Why Do We Need NAT?

- Conserves public IPv4 addresses
- Allows private networks to communicate with the Internet
- Provides an additional layer of security by hiding internal IP addresses
- Reduces the need for multiple public IP addresses

---

## 🌐 Private IP Address Ranges

| Class | Range |
|--------|----------------------|
| A | 10.0.0.0 – 10.255.255.255 |
| B | 172.16.0.0 – 172.31.255.255 |
| C | 192.168.0.0 – 192.168.255.255 |

---

## 🌍 Public IP Address

A Public IP address is assigned by an Internet Service Provider (ISP) and is globally unique.

Example:
- 8.8.8.8
- 1.1.1.1

---

# Types of NAT

## 1. Static NAT

- One Private IP ↔ One Public IP
- Permanent mapping
- Used for servers

Example:

192.168.1.10 ↔ 203.0.113.10

---

## 2. Dynamic NAT

- Maps private IPs to a pool of public IPs
- Temporary mapping
- Public IP assigned dynamically

---

## 3. PAT (Port Address Translation)

Also called NAT Overload.

- Multiple private IPs share one public IP
- Uses different port numbers
- Most commonly used in homes and offices

Example:

192.168.1.10:1025 → 203.0.113.1:3001

192.168.1.20:1026 → 203.0.113.1:3002

---

# NAT Terminology

## Inside Local

Private IP address inside the LAN.

Example:
192.168.1.10

---

## Inside Global

Public IP representing the inside device.

Example:
203.0.113.1

---

## Outside Global

Public IP address of the external destination.

Example:
8.8.8.8

---

## Outside Local

External address as seen from the internal network.

Usually the same as the Outside Global address.

---

# Advantages of NAT

- Conserves IPv4 addresses
- Hides internal network
- Improves security
- Easy Internet access for private networks
- Cost-effective

---

# Disadvantages of NAT

- Increases processing on the router
- Makes troubleshooting more difficult
- Some applications require additional NAT configuration

---

# Cisco Commands

```bash
show ip nat translations
show ip nat statistics
show running-config
show ip interface brief
```

---

# Verification Commands

```bash
ping
show ip nat translations
show ip nat statistics
```

---

# Interview Questions

### 1. What is NAT?

NAT translates private IP addresses into public IP addresses to enable Internet communication.

---

### 2. Why is NAT required?

To conserve public IP addresses and allow private networks to access the Internet.

---

### 3. Difference between Static NAT and Dynamic NAT?

| Static NAT | Dynamic NAT 
|-------------|-------------|
| One-to-One | Uses Public IP Pool |
| Permanent Mapping | Temporary Mapping |

---

### 4. What is PAT?

PAT allows multiple devices to share a single public IP address using different port numbers.

---

### 5. Which NAT type is commonly used in homes?

PAT (Port Address Translation)

---

# Summary

- NAT translates Private IP ↔ Public IP.
- Static NAT uses one public IP per private IP.
- Dynamic NAT uses a pool of public IP addresses.
- PAT allows multiple devices to share one public IP using port numbers.
- NAT helps conserve IPv4 addresses and improves network security.

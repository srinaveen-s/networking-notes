# DNS (Domain Name System)

## 📖 What is DNS?

Domain Name System (DNS) is a network service that translates human-readable domain names (such as **www.google.com**) into IP addresses that computers use to communicate over a network.

---

## 🎯 Why Do We Need DNS?

- Converts domain names into IP addresses
- Makes websites easier to access
- Eliminates the need to remember IP addresses
- Speeds up network communication through caching
- Supports internet and private network services

---

# How DNS Works

1. The user enters a domain name (e.g., www.example.com).
2. The DNS client sends a query to the DNS server.
3. The DNS server searches for the matching record.
4. The DNS server returns the corresponding IP address.
5. The client connects to the destination server using the IP address.

---

# DNS Resolution Process

- User enters a domain name.
- DNS Resolver receives the request.
- Root DNS Server is queried.
- Top-Level Domain (TLD) Server is queried.
- Authoritative DNS Server provides the IP address.
- The client connects to the destination.

---

# Common DNS Record Types

## A Record

Maps a domain name to an IPv4 address.

Example:

```text
www.company.local → 192.168.1.100
```

---

## AAAA Record

Maps a domain name to an IPv6 address.

---

## CNAME Record

Creates an alias for another domain name.

Example:

```text
mail.company.local → server.company.local
```

---

## MX Record

Specifies the mail server for a domain.

---

## NS Record

Identifies the authoritative DNS server for a domain.

---

## PTR Record

Used for reverse DNS lookup (IP address to domain name).

---

# DNS Hierarchy

- Root DNS Server
- Top-Level Domain (TLD) Server
- Authoritative DNS Server
- Client

---

# Cisco DNS Commands

Configure DNS lookup:

```bash
ip domain-lookup
```

Configure a DNS server:

```bash
ip name-server 192.168.1.2
```

Configure a domain name:

```bash
ip domain-name company.local
```

---

# Verification Commands

```bash
show hosts

ping www.company.local
```

---

# Advantages

- Easy access using domain names
- Eliminates the need to remember IP addresses
- Supports hierarchical naming
- Improves scalability
- Supports caching for faster lookups

---

# Limitations

- DNS server failure can affect name resolution
- Incorrect records cause connectivity issues
- DNS cache poisoning attacks are possible
- Requires proper server configuration

---

# Interview Questions

### 1. What is DNS?

DNS is a naming service that translates domain names into IP addresses.

---

### 2. Which port does DNS use?

Port **53** (UDP and TCP).

---

### 3. What is an A Record?

It maps a domain name to an IPv4 address.

---

### 4. What is an AAAA Record?

It maps a domain name to an IPv6 address.

---

### 5. What is an MX Record?

It specifies the mail server for a domain.

---

### 6. What is a CNAME Record?

It creates an alias for another domain name.

---

### 7. What is a PTR Record?

It is used for reverse DNS lookup.

---

### 8. Which command configures a DNS server on a Cisco router?

```bash
ip name-server 192.168.1.2
```

---

### 9. Which port does DNS primarily use?

UDP Port **53**.

---

### 10. Why is DNS important?

DNS allows users to access resources using easy-to-remember domain names instead of IP addresses.

---

# Summary

- DNS translates domain names into IP addresses.
- DNS uses Port 53.
- DNS improves usability and scalability.
- Common records include A, AAAA, CNAME, MX, NS, and PTR.
- DNS is an essential service in modern computer networks.

---

# 👨‍💻 Author

**Srinaveen S**

Passionate Electronics and Communication Engineering student with a strong interest in Computer Networks, Cisco Networking, and Network Security. This documentation was created as part of my hands-on networking practice to strengthen practical networking skills using Cisco Packet Tracer.

# Access Control List (ACL)

## 📖 What is an Access Control List (ACL)?

An Access Control List (ACL) is a set of rules used on Cisco routers and switches to control network traffic. ACLs allow or deny packets based on conditions such as source IP address, destination IP address, protocol, or port number.

---

## 🎯 Why Do We Need ACL?

- Controls network traffic
- Improves network security
- Restricts unauthorized access
- Filters incoming and outgoing packets
- Protects network resources

---

# Types of ACL

## 1. Standard ACL

- Filters traffic based only on the source IP address.
- Uses ACL numbers 1–99 and 1300–1999.
- Usually placed close to the destination.

Example:

```bash
access-list 10 permit 192.168.1.0 0.0.0.255
```

---

## 2. Extended ACL

- Filters traffic based on source IP, destination IP, protocol, and port numbers.
- Uses ACL numbers 100–199 and 2000–2699.
- Usually placed close to the source.

Example:

```bash
access-list 100 permit tcp 192.168.1.0 0.0.0.255 any eq 80
```

---

# ACL Rules

- ACLs are processed from top to bottom.
- The first matching rule is applied.
- Every ACL has an implicit "deny all" at the end.
- Order of ACL entries is important.

---

# Wildcard Mask

A wildcard mask tells the router which bits of an IP address should be checked.

Examples:

| Subnet Mask | Wildcard Mask |
|--------------|---------------|
|255.255.255.0 |0.0.0.255|
|255.255.0.0|0.0.255.255|
|255.0.0.0|0.255.255.255|

---

# Standard ACL Commands

```bash
access-list 10 permit 192.168.1.0 0.0.0.255

interface GigabitEthernet0/0

ip access-group 10 in
```

---

# Extended ACL Commands

```bash
access-list 100 permit tcp any any eq 80

interface GigabitEthernet0/0

ip access-group 100 in
```

---

# Verification Commands

```bash
show access-lists

show running-config

show ip interface
```

---

# Advantages

- Enhances network security
- Controls user access
- Reduces unwanted traffic
- Easy to configure
- Improves network performance

---

# Limitations

- Incorrect rule order may block valid traffic.
- Standard ACL filters only by source IP.
- Large ACLs can be difficult to manage.

---

# Interview Questions

### 1. What is ACL?

ACL is a set of rules used to permit or deny network traffic.

---

### 2. What are the two types of ACL?

- Standard ACL
- Extended ACL

---

### 3. What does a Standard ACL filter?

Only the source IP address.

---

### 4. What does an Extended ACL filter?

Source IP, destination IP, protocol, and port number.

---

### 5. What is the default action at the end of every ACL?

Implicit Deny All.

---

### 6. Where should a Standard ACL be placed?

Close to the destination.

---

### 7. Where should an Extended ACL be placed?

Close to the source.

---

### 8. Which command displays ACL entries?

```bash
show access-lists
```

---

### 9. What is a wildcard mask?

A wildcard mask specifies which bits of an IP address should be matched during ACL processing.

---

### 10. Why are ACLs important?

ACLs improve network security by controlling and filtering network traffic.

---

# Summary

- ACL controls network traffic by permitting or denying packets.
- Standard ACL filters only source IP addresses.
- Extended ACL filters source IP, destination IP, protocol, and port numbers.
- Every ACL ends with an implicit deny statement.
- ACLs are widely used to improve network security and traffic management.

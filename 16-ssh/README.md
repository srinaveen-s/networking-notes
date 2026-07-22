# SSH (Secure Shell)

## 📖 What is SSH?

SSH (Secure Shell) is a secure network protocol used to remotely access and manage network devices over an encrypted connection. It provides secure communication between a client and a server, replacing the insecure Telnet protocol.

---

## 🎯 Why Do We Need SSH?

- Provides secure remote access to network devices
- Encrypts usernames, passwords, and data
- Protects against eavesdropping and unauthorized access
- Allows secure network administration
- Replaces Telnet for device management

---

# SSH vs Telnet

| SSH | Telnet |
|------|--------|
| Encrypted communication | Plain text communication |
| Secure | Not Secure |
| Uses Port 22 | Uses Port 23 |
| Recommended for production | Not recommended |

---

# How SSH Works

1. The client requests a secure connection to the server.
2. The server authenticates the client.
3. RSA keys are used to establish an encrypted session.
4. The user logs in with a username and password.
5. All communication is securely encrypted.

---

# Requirements for SSH

- Hostname configured
- Domain name configured
- Local username and password
- RSA keys generated
- SSH Version 2 enabled
- VTY lines configured

---

# Cisco Configuration Commands

```bash
hostname R1

ip domain-name lab.local

username admin secret Cisco123

crypto key generate rsa

1024

ip ssh version 2

line vty 0 4

login local

transport input ssh
```

---

# Verification Commands

```bash
show ip ssh

show ssh

show running-config
```

To connect from a PC:

```bash
ssh -l admin 192.168.1.1
```

---

# Advantages

- Secure remote device management
- Encrypts sensitive information
- Supports user authentication
- Prevents password theft
- Widely used in enterprise networks

---

# Limitations

- Initial configuration is required
- Slightly more CPU intensive than Telnet
- Requires RSA key generation
- More complex than Telnet for beginners

---

# Interview Questions

### 1. What is SSH?

SSH is a secure protocol used for remote login and network device management.

---

### 2. Which port does SSH use?

Port **22**.

---

### 3. Which port does Telnet use?

Port **23**.

---

### 4. Why is SSH more secure than Telnet?

SSH encrypts all communication, while Telnet sends data in plain text.

---

### 5. Which command generates RSA keys?

```bash
crypto key generate rsa
```

---

### 6. Which command enables SSH Version 2?

```bash
ip ssh version 2
```

---

### 7. Which command configures a local user?

```bash
username admin secret Cisco123
```

---

### 8. Which command allows only SSH on VTY lines?

```bash
transport input ssh
```

---

### 9. Which command verifies SSH status?

```bash
show ip ssh
```

---

### 10. Why is SSH important?

SSH provides secure remote access and protects network devices from unauthorized access.

---

# Summary

- SSH is a secure remote access protocol.
- SSH encrypts all communication between client and server.
- SSH uses Port 22.
- RSA keys are required for encrypted communication.
- SSH is the recommended method for remote network device management.

---

# 👨‍💻 Author

**Srinaveen S**

Passionate Electronics and Communication Engineering student with a strong interest in Computer Networks, Cisco Networking, and Network Security. This documentation was created as part of my hands-on networking practice to strengthen practical networking skills using Cisco Packet Tracer.

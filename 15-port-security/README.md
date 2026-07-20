# Port Security

## 📖 What is Port Security?

Port Security is a Layer 2 security feature on Cisco switches that restricts access to a switch port by allowing only specific MAC addresses to connect. It helps prevent unauthorized devices from accessing the network.

---

## 🎯 Why Do We Need Port Security?

- Prevents unauthorized network access
- Improves network security
- Protects against MAC flooding attacks
- Restricts unknown devices from connecting
- Enhances access control

---

# How Port Security Works

Port Security allows a switch port to learn or manually configure MAC addresses. If an unauthorized device connects to the port, the configured violation action is triggered.

---

# Violation Modes

## 1. Protect

- Drops packets from unauthorized devices.
- No log or notification is generated.
- Port remains active.

---

## 2. Restrict

- Drops packets from unauthorized devices.
- Generates logs and increments the violation counter.
- Port remains active.

---

## 3. Shutdown

- Default violation mode.
- Port changes to the Err-Disabled state.
- Requires manual or automatic recovery.

---

# Sticky MAC Address

Sticky MAC allows the switch to automatically learn MAC addresses and save them in the running configuration.

Example:

```bash
switchport port-security mac-address sticky
```

---

# Maximum MAC Address

Specifies the maximum number of MAC addresses allowed on a switch port.

Example:

```bash
switchport port-security maximum 1
```

---

# Cisco Configuration Commands

```bash
interface FastEthernet0/1

switchport mode access

switchport port-security

switchport port-security maximum 1

switchport port-security mac-address sticky

switchport port-security violation shutdown
```

---

# Verification Commands

```bash
show port-security

show port-security interface fastEthernet0/1

show running-config
```

---

# Advantages

- Prevents unauthorized access
- Improves Layer 2 security
- Supports Sticky MAC learning
- Easy to configure
- Protects switch ports

---

# Limitations

- Only works on access ports
- Requires proper configuration
- Port may become Err-Disabled in Shutdown mode
- Not suitable for ports connected to multiple users

---

# Interview Questions

### 1. What is Port Security?

Port Security is a Cisco switch feature that restricts access to a switch port based on MAC addresses.

---

### 2. Which layer does Port Security operate on?

Layer 2 (Data Link Layer).

---

### 3. What are the three violation modes?

- Protect
- Restrict
- Shutdown

---

### 4. What is the default violation mode?

Shutdown.

---

### 5. What is Sticky MAC?

Sticky MAC automatically learns and stores MAC addresses on a secure port.

---

### 6. Which command enables Port Security?

```bash
switchport port-security
```

---

### 7. Which command sets the maximum number of MAC addresses?

```bash
switchport port-security maximum 1
```

---

### 8. Which command enables Sticky MAC?

```bash
switchport port-security mac-address sticky
```

---

### 9. Which command displays Port Security information?

```bash
show port-security
```

---

### 10. Why is Port Security important?

It prevents unauthorized devices from connecting to the network and improves Layer 2 security.

---

# Summary

- Port Security protects switch ports from unauthorized devices.
- It works by allowing only specified MAC addresses.
- Sticky MAC automatically learns MAC addresses.
- Violation modes include Protect, Restrict, and Shutdown.
- Port Security is an important Layer 2 security feature in Cisco networks.
- ---

# 👨‍💻 Author

**Srinaveen S**

Passionate Electronics and Communication Engineering student with a strong interest in Computer Networks, Cisco Networking, and Network Security. This documentation was created as part of my hands-on networking practice to strengthen practical networking skills using Cisco Packet Tracer.

---

# RIP (Routing Information Protocol)

> **Status:** ✅ Completed

---

## 📖 Overview

Routing Information Protocol (RIP) is a dynamic routing protocol that automatically exchanges routing information between routers. It uses **Hop Count** as the routing metric to determine the best path to a destination network.

Unlike Static Routing, RIP automatically updates routing tables whenever network changes occur.

---

## 🎯 Why is RIP Needed?

RIP helps to:

- Automatically exchange routing information
- Reduce manual configuration
- Automatically update routes when the network changes
- Simplify network management

---

## 🌐 How RIP Works

Each router periodically shares its routing table with neighboring routers.

When a router receives new routing information, it updates its routing table if a better path is available.

The route with the **lowest hop count** is selected as the best path.

---

## 📚 RIP Versions

### RIP Version 1 (RIPv1)

- Classful routing protocol
- Does not support VLSM
- Uses Broadcast updates

### RIP Version 2 (RIPv2)

- Classless routing protocol
- Supports VLSM and CIDR
- Uses Multicast (224.0.0.9)
- Supports Authentication

---

## 📏 Hop Count

Hop Count is the number of routers a packet passes through before reaching its destination.

Example:

PC1 → R1 → R2 → R3 → PC2

Hop Count = 3

Maximum Hop Count = **15**

A route with **16 hops** is considered unreachable.

---

## 🌍 Real-World Example

A company has multiple branch offices connected through several routers.

Instead of manually configuring routes on every router, RIP automatically exchanges routing information between routers so that all branch offices can communicate with each other.

---

## 📦 Advantages

- Easy to configure
- Automatic route updates
- Suitable for small networks
- Low administrative effort

---

## ⚠️ Disadvantages

- Slow convergence
- Maximum of 15 hops
- Not suitable for large networks
- Less efficient than OSPF

---

## 💼 Interview Questions

- What is RIP?
- What metric does RIP use?
- What is the maximum hop count in RIP?
- What is the difference between RIPv1 and RIPv2?
- Why is RIP called a dynamic routing protocol?

---

## 📝 Verification Commands

```text
show ip route

show ip protocols

show running-config
```

---

## 📝 What I Learned

After learning RIP, I understood how routers automatically exchange routing information without manually configuring static routes. I also learned the importance of hop count, RIP Version 2, and how dynamic routing simplifies network management.

---

## 👨‍💻 Author

**SRINAVEEN S**

BE Electronics and Communication Engineering

Building My Network Engineering Portfolio

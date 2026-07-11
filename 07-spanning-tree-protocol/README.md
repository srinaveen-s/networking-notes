# Spanning Tree Protocol (STP)

> **Status:** ✅ Completed

---

## 📖 Overview

Spanning Tree Protocol (STP) is a Layer 2 network protocol that prevents switching loops in Ethernet networks. It automatically blocks redundant paths while keeping them available as backup links.

STP was developed to improve network reliability and prevent broadcast storms caused by network loops.

---

## 🎯 Why is STP Needed?

Without STP, connecting switches with multiple redundant links can create loops. These loops may cause:

- Broadcast Storms
- Multiple Frame Copies
- MAC Address Table Instability
- Network Congestion

STP detects these loops and blocks unnecessary paths while keeping the network operational.

---

## 🌐 How STP Works

STP elects one switch as the **Root Bridge**.

Each switch calculates the shortest path to the Root Bridge.

If multiple paths exist, STP blocks one of the redundant paths to prevent loops.

If the active path fails, the blocked path automatically becomes active.

---

## 📚 Important STP Terms

### Root Bridge

The main switch selected by STP to serve as the reference point for the network.

---

### Root Port

The port on a switch that provides the shortest path to the Root Bridge.

---

### Designated Port

The forwarding port selected for each network segment.

---

### Blocking Port

A redundant port that is placed in the blocking state to prevent network loops.

---

## 🌍 Real-World Example

A company connects three switches together for redundancy.

If one cable fails, the backup cable keeps the network running.

Without STP, both cables would forward traffic and create loops.

With STP enabled, one link remains active while the other stays in the blocking state until needed.

---

## 📦 Advantages of STP

- Prevents Network Loops
- Avoids Broadcast Storms
- Improves Network Stability
- Supports Redundant Links
- Provides Automatic Failover

---

## 💼 Interview Questions

- What is STP?
- Why is STP used?
- What is a Root Bridge?
- What is a Blocking Port?
- What is a Broadcast Storm?
- Which OSI Layer does STP operate on?

---

## 📝 What I Learned

After learning STP, I understood how switches prevent network loops by electing a Root Bridge and blocking redundant links. I also learned why STP is an important protocol for building reliable and stable Ethernet networks.

---

## 👨‍💻 Author

SRINAVEEN S

BE Electronics and Communication Engineering

Building My Network Engineering Portfolio

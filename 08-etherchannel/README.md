# EtherChannel

> **Status:** ✅ Completed

---

## 📖 Overview

EtherChannel is a Layer 2 technology that combines multiple physical Ethernet links into a single logical link. It increases bandwidth, provides redundancy, and improves network reliability.

Instead of using one cable between two switches, EtherChannel allows multiple cables to work together as a single connection.

---

## 🎯 Why is EtherChannel Needed?

Using a single cable between switches can create a bottleneck and a single point of failure.

EtherChannel helps to:

- Increase available bandwidth.
- Provide link redundancy.
- Improve network performance.
- Reduce the impact of link failures.
- Simplify network management.

---

## 🌐 How EtherChannel Works

EtherChannel groups multiple physical interfaces into one logical interface called a **Port-Channel**.

Traffic is distributed across the member links, and if one link fails, the remaining links continue to carry traffic without interrupting network communication.

---

## 📚 EtherChannel Protocols

### LACP (Link Aggregation Control Protocol)

- IEEE Standard: 802.3ad (802.1AX)
- Open standard
- Works with devices from different vendors
- Modes: Active and Passive

---

### PAgP (Port Aggregation Protocol)

- Cisco proprietary protocol
- Works only on Cisco devices
- Modes: Desirable and Auto

---

## 🌍 Real-World Example

A company has two switches connected with multiple network cables.

Instead of using only one cable, EtherChannel combines multiple cables into one logical connection. This increases bandwidth and keeps the network running even if one cable fails.

---

## 📦 Advantages of EtherChannel

- Higher Bandwidth
- Link Redundancy
- Load Balancing
- Improved Reliability
- Easier Network Management

---

## 💼 Interview Questions

- What is EtherChannel?
- Why is EtherChannel used?
- What is the difference between LACP and PAgP?
- What is a Port-Channel?
- What happens if one link in an EtherChannel fails?

---

## 📝 What I Learned

After learning EtherChannel, I understood how multiple physical links can be combined into one logical connection to improve bandwidth, provide redundancy, and increase network reliability.

I also learned the difference between LACP and PAgP and how EtherChannel works with a Port-Channel interface.

---

## 👨‍💻 Author

SRINAVEEN S

BE Electronics and Communication Engineering

Building My Network Engineering Portfolio

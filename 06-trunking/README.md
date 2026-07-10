# Trunking

> **Status:** ✅ Completed

---

## 📖 Overview

Trunking is a networking technique that allows multiple VLANs to pass through a single physical link between network devices, such as switches or a switch and a router.

Instead of using separate cables for each VLAN, one trunk link can carry traffic from multiple VLANs.

---

## 🎯 Why is Trunking Needed?

Without trunking, each VLAN would require a separate physical connection between switches.

Trunking allows:

- Multiple VLANs to share a single cable.
- Efficient use of network ports.
- Easier network expansion.
- Better network management.

---

## 🌐 How Trunking Works

A trunk port carries traffic from multiple VLANs.

Each Ethernet frame is tagged with a VLAN ID using the IEEE 802.1Q standard so that the receiving device knows which VLAN the frame belongs to.

---

## 📦 Access Port vs Trunk Port

**Access Port**

- Belongs to only one VLAN.
- Usually connected to end devices like PCs or printers.

**Trunk Port**

- Carries traffic from multiple VLANs.
- Usually connected between switches or between a switch and a router.

---

## 🏢 Real-World Example

Imagine a company with three departments:

- HR (VLAN 10)
- Finance (VLAN 20)
- IT (VLAN 30)

Two switches are connected together.

Instead of using three separate cables between the switches, a single trunk link carries traffic for all three VLANs.

---

## 📘 IEEE Standard

Trunking uses the IEEE 802.1Q standard to identify VLAN information inside Ethernet frames.

---

## 💼 Interview Questions

- What is trunking?
- Why is trunking used?
- What is an access port?
- What is a trunk port?
- What is IEEE 802.1Q?

---

## 📝 What I Learned

After learning trunking, I understood how multiple VLANs can communicate across switches using a single physical connection. I also learned the difference between access ports and trunk ports.

---

## 👨‍💻 Author

SRINAVEEN S

BE Electronics and Communication Engineering

Building My Network Engineering Portfolio

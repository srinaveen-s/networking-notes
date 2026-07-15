# OSPF (Open Shortest Path First)

> **Status:** ✅ Completed

---

## 📖 Overview

Open Shortest Path First (OSPF) is a dynamic link-state routing protocol used to exchange routing information between routers. It calculates the best path using the **Shortest Path First (SPF)** algorithm and uses **Cost** as its routing metric.

OSPF is faster, more scalable, and more efficient than RIP, making it one of the most widely used routing protocols in enterprise networks.

---

## 🎯 Why is OSPF Needed?

OSPF helps to:

- Automatically exchange routing information
- Quickly adapt to network changes
- Support large enterprise networks
- Find the shortest and best path to a destination
- Reduce manual route configuration

---

## 🌐 How OSPF Works

OSPF routers first discover their neighboring routers and establish neighbor relationships.

They then exchange routing information and build a complete network topology database.

Finally, OSPF uses the **Shortest Path First (SPF)** algorithm to calculate the best route.

---

## 📚 OSPF Terminology

### Router ID

A unique identifier assigned to every OSPF router.

### Area

OSPF divides large networks into areas.

The backbone area is:

```text
Area 0
```

### Cost

OSPF selects the best path based on **Cost**.

Lower Cost = Better Path

### Neighbor

Routers running OSPF become neighbors before exchanging routing information.

---

## 🌍 Real-World Example

A company has multiple branch offices connected through several routers.

Instead of manually configuring routes on every router, OSPF automatically exchanges routing information and calculates the shortest path for data transmission.

---

## 📦 Advantages

- Fast convergence
- Supports large networks
- Classless routing protocol
- Supports VLSM and CIDR
- Efficient routing updates
- Scalable and reliable

---

## ⚠️ Disadvantages

- More complex than RIP
- Requires more CPU and memory
- Configuration is slightly difficult for beginners

---

## 🔄 OSPF vs RIP

| RIP | OSPF |
|-----|------|
| Distance Vector | Link State |
| Metric: Hop Count | Metric: Cost |
| Slow convergence | Fast convergence |
| Maximum 15 hops | No hop limit |
| Suitable for small networks | Suitable for medium and large networks |

---

## 💼 Interview Questions

- What is OSPF?
- What routing algorithm does OSPF use?
- What metric does OSPF use?
- What is Area 0?
- What is Router ID?
- Difference between RIP and OSPF?

---

## 📝 Verification Commands

```text
show ip ospf neighbor

show ip route

show ip protocols

show running-config
```

---

## 📝 What I Learned

After learning OSPF, I understood how routers automatically discover neighbors, exchange routing information, and calculate the shortest path using the SPF algorithm. I also learned why OSPF is preferred over RIP in enterprise networks.

---

## 👨‍💻 Author

**SRINAVEEN S**

BE Electronics and Communication Engineering

Building My Network Engineering Portfolio

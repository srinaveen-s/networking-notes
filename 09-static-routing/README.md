# Static Routing

> **Status:** ✅ Completed

---

## 📖 Overview

Static Routing is a method of manually configuring routes on a router to allow communication between different networks. The network administrator specifies the path that packets should follow to reach a destination network.

Unlike dynamic routing protocols, static routes do not update automatically when the network topology changes.

---

## 🎯 Why is Static Routing Needed?

Routers only know about directly connected networks. To communicate with remote networks, they need routing information.

Static Routing helps to:

- Connect different networks.
- Control the exact path of network traffic.
- Improve security by allowing only specific routes.
- Reduce routing overhead.
- Build small and stable networks.

---

## 🌐 How Static Routing Works

A network administrator manually configures routes using the destination network, subnet mask, and next-hop IP address.

When a router receives a packet, it checks its routing table and forwards the packet through the configured route.

---

## 📚 Static Route Syntax

```text
ip route <destination-network> <subnet-mask> <next-hop-ip>
```

Example:

```text
ip route 192.168.2.0 255.255.255.0 10.0.0.2
```

This route tells the router to send all traffic destined for the **192.168.2.0/24** network to the next-hop router at **10.0.0.2**.

---

## 🌍 Real-World Example

A company has two branch offices connected by two routers.

- Branch A Network: 192.168.1.0/24
- Branch B Network: 192.168.2.0/24

Static routes are configured on both routers so that users in each branch can communicate with the other branch.

---

## 📦 Advantages of Static Routing

- Easy to configure in small networks
- Low CPU and memory usage
- Better security
- Full control over routing paths
- No routing protocol traffic

---

## ⚠️ Disadvantages

- Manual configuration required
- Not suitable for large networks
- Routes must be updated manually if the network changes
- Difficult to manage in complex environments

---

## 💼 Interview Questions

- What is Static Routing?
- Why is Static Routing used?
- What is the syntax of a static route?
- What is a next-hop IP address?
- What is the difference between Static Routing and Dynamic Routing?

---

## 📝 What I Learned

After learning Static Routing, I understood how routers communicate with remote networks using manually configured routes. I also learned how to configure static routes, verify the routing table, and understand the role of the next-hop IP address in packet forwarding.

---

## 👨‍💻 Author

SRINAVEEN S

BE Electronics and Communication Engineering

Building My Network Engineering Portfolio

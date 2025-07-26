# CNG-21x1: Networking Foundations Lab

Welcome to **CNG-21x1**, a 14-week hands-on course in networking fundamentals using open-source tools. This course introduces the core protocols, architectures, and operations that power modern computer networks — from Ethernet and IP to BGP and MPLS. All labs are built using [Containerlab](https://containerlab.dev/) and run locally using containerized routers.

---

## 📚 Course Description

This course explores how data moves through networks using real topologies, emulated routers, and open-source tools. You will design, deploy, and troubleshoot Layer 2 and Layer 3 networks, learn routing protocols, and understand the structure of the Internet. 

Every week includes:
- A reading and historical context piece
- A Containerlab-based lab
- A short comic or lesson from **Ned**, our fictional junior engineer who makes classic mistakes

This course is **open source** and hosted entirely on GitHub.

---

## 🛠️ Lab Environment

We use the following tools:
- [Containerlab](https://containerlab.dev/)
- [Docker](https://www.docker.com/)
- [Wireshark](https://www.wireshark.org/)
- [Git](https://git-scm.com/) and GitHub

All topologies are defined using `clab.yml` files. You’ll clone this repo, launch labs with `containerlab deploy`, and use CLI + packet tools to debug real protocol interactions.

---

## 🧠 Weekly Topics

| Week | Topic                              | Lab |
|------|------------------------------------|-----|
| 1    | Introduction + Lab Setup           | 2-node ping + tcpdump |
| 2    | Ethernet & MAC Learning            | L2 switch fabric |
| 3    | VLANs & Trunking                   | VLAN separation + router-on-a-stick |
| 4    | Spanning Tree Protocol             | Redundant L2 + STP convergence |
| 5    | IPv4 Addressing & Subnetting       | Multi-subnet IP plan |
| 6    | ARP, DHCP, and ICMP                | Relay + Wireshark analysis |
| 7    | Routing I: OSPF                    | Multi-area topology |
| 8    | Routing II: IS-IS                  | L1/L2 domains |
| 9    | BGP Fundamentals                   | eBGP peering |
| 10   | BGP Policy & Attributes            | Route-maps, AS-path |
| 11   | MPLS & Label Switching             | LSP + traceroute |
| 12   | Layer 3 VPNs (MPLS)                | PE-CE VRFs |
| 13   | EVPN + VXLAN                       | Overlay bridge domain |
| 14   | Capstone Project                   | Full topology design |

---

## 📁 Repository Structure

```
.
├── labs/
│   ├── week01/
│   ├── week02/
│   └── ...
├── docs/
│   ├── syllabus.md
│   ├── learning-objectives.md
│   └── references.md
├── ned/
│   └── week01.png
├── scripts/
│   └── helper-tools.sh
├── .gitignore
└── README.md
```

---

## 🧅 Philosophy: Networks Have Layers

Like ogres (and onions), networks are built in **layers**. You'll learn both the OSI and DoD (TCP/IP) models as part of this class. This layered approach helps explain how Ethernet, IP, TCP/UDP, and apps all interact.

> *“Networks are like onions. They have layers.”* — Probably Shrek if he were a network engineer

---

## 🔧 Getting Started

1. Install Docker
2. Install Containerlab
3. Clone this repo:
   ```bash
   git clone https://github.com/YOUR-ORG/CNG-21x1.git
   cd CNG-21x1
   ```
4. Run your first lab:
   ```bash
   cd labs/week01
   containerlab deploy -t lab01.clab.yml
   ```

---

## 🙃 Meet Ned

Each week features **Ned**, our fictional junior network engineer. Ned forgets to save configs, plugs cables into loopbacks, and deletes BGP sessions in production. Learn from Ned’s mishaps in the “Ned’s Corner” section of each lab.

---

## 📖 License

This course is open source under the [MIT License](LICENSE).

---

## 🧵 Contributions

Pull requests welcome! If you spot a typo, want to improve a lab, or add new historical content, we’d love your help.

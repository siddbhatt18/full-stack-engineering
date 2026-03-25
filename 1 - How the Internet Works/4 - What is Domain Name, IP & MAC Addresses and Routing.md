Here’s a Phase‑1 level, but still detailed, tutorial on:

# Domain Names, IP & MAC Addresses, and Routing

These are core building blocks of “how the internet works.” Once you understand them, almost everything else (DNS, HTTP, hosting, etc.) will feel much easier.

We’ll cover:

1. Why we need these identifiers  
2. Domain names  
3. IP addresses (IPv4, IPv6, public vs private)  
4. MAC addresses  
5. How they work together  
6. What routing is and how it works at a high level  

---

## 1. Why So Many “Addresses”?

On the internet, your data might travel:

- From your laptop → Wi‑Fi router → ISP → many routers → data center → server.

At each stage, the network needs a way to know:

- **Which machine** to send to (globally) → IP address  
- **Which device on a local network** → MAC address  
- **Which human‑friendly name** we’re talking about → domain name (like `google.com`)  

Different layers of the network use **different kinds of addresses**, for different scopes:

- **MAC**: “Who is this network card?” (local link only)  
- **IP**: “Where is this device on the internet / network?” (global routing)  
- **Domain name**: “What website/service does the human want?” (human layer)  

Routing glues it all together: **how to move packets from one IP to another, across many networks.**

---

## 2. Domain Names

### 2.1 What is a domain name?

A **domain name** is a human‑friendly identifier for an internet resource, like a website or service:

- Examples:
  - `google.com`
  - `github.com`
  - `example.org`
  - `my-portfolio.dev`

Computers actually care about **IP addresses**, not names. Domain names are for people. We use **DNS (Domain Name System)** to translate a domain name into an IP address.

### 2.2 Domain name structure

Take `www.example.com`:

- `.` – implicit root of the DNS tree  
- `com` – **Top-Level Domain (TLD)**  
- `example` – **Second-Level Domain** (owned by some organization/person)  
- `www` – **Subdomain**  

More examples:

- `api.example.com` → subdomain `api` of `example.com`  
- `blog.mycompany.co.in`  
  - TLD: `in`  
  - Second‑level: `co`  
  - Third‑level: `mycompany`  
  - Subdomain: `blog`

### 2.3 How domains are managed

- Domains are registered via **domain registrars** (e.g., Namecheap, GoDaddy, Google Domains).
- When you buy `mycoolsite.com`, you:
  - Become its owner (for the registration period).
  - Configure **DNS records** (A, AAAA, CNAME, etc.) to point it to server IPs.

### 2.4 DNS: Mapping domain → IP

When you enter `https://example.com` in your browser:

1. Browser checks local DNS cache.
2. If not found, it asks a **DNS resolver** (usually provided by your ISP or something like 8.8.8.8 from Google).
3. Resolver finds the IP address (e.g., `93.184.216.34`) by querying DNS servers.
4. Browser then talks to `93.184.216.34` using HTTP/HTTPS.

So:

- **Domain name** is like: `myfriend.com` (name in your contacts).
- **IP address** is like: `+91-98765-43210` (actual phone number the network dials).

---

## 3. IP Addresses (Internet Protocol Addresses)

An **IP address** identifies a device on a network that uses the Internet Protocol. Routers use IP addresses to deliver data between networks.

### 3.1 IPv4 vs IPv6

**IPv4** (most common today):

- Written as four numbers (0–255) separated by dots.
- Example: `192.168.1.10`, `8.8.8.8`
- 32‑bit address → about 4.3 billion possible addresses (not enough for every device worldwide).

**IPv6** (newer, larger address space):

- Written as eight groups of hexadecimal numbers separated by colons.
- Example: `2001:0db8:85a3:0000:0000:8a2e:0370:7334`
- 128‑bit address → astronomically more addresses (designed to solve IPv4 exhaustion).

At Phase 1, it’s enough to:

- Recognize IPv4: `x.x.x.x`
- Know IPv6 exists and is longer with `:`.

### 3.2 Public vs Private IP addresses

**Public IP address**:

- Globally unique on the internet.
- Assigned to:
  - Your **router** by your ISP.
  - Servers in data centers.
- Example: `8.8.8.8` (Google DNS), `13.107.42.14` (a Microsoft server, for example).

**Private IP address**:

- Used inside local networks (LAN).
- Not routable on the public internet directly.
- Reserved ranges (IPv4):
  - `10.0.0.0` – `10.255.255.255`
  - `172.16.0.0` – `172.31.255.255`
  - `192.168.0.0` – `192.168.255.255`
- Examples: `192.168.1.10`, `10.0.0.5`

Your home network:

- Router gets one **public IP** from ISP (e.g., `122.160.45.23`).
- Router gives your devices **private IPs**:
  - Laptop: `192.168.1.10`
  - Phone: `192.168.1.11`
  - TV: `192.168.1.12`

Router uses **NAT (Network Address Translation)** so all these devices can share the single public IP when talking to the internet.

### 3.3 What does IP actually do?

IP is responsible for:

- **Addressing**: identifying the source and destination.
- **Routing** packets between different networks.
- IP packets carry:
  - Source IP address
  - Destination IP address
  - Other info (TTL, protocol, etc.)
  - Payload (TCP/UDP data)

IP is **unreliable** and **best-effort**:

- It doesn’t guarantee delivery, order, or no duplication.
- Reliability is handled by **TCP** (or at application layer).

---

## 4. MAC Addresses (Media Access Control Addresses)

A **MAC address** is a low‑level, hardware identifier for a **network interface card (NIC)**.

### 4.1 What is a MAC address?

- Assigned by the NIC manufacturer (can sometimes be changed in software).
- Typically 48 bits, written as 6 groups of 2 hex digits:
  - `00:1A:2B:3C:4D:5E`
  - `F0-9F-C2-3E-4A-11`

Every network device (your laptop’s Wi‑Fi card, your router’s Ethernet port, etc.) has **at least one** MAC address.

### 4.2 Where MAC addresses are used

- Used in **local networks (LAN)** at the **Link Layer** (Ethernet/Wi‑Fi).
- Devices in the same LAN communicate with **frames** that contain:
  - Source MAC
  - Destination MAC
- Switches use MAC addresses to know which port a device is on.

Example:

- Your laptop needs to send a packet to your router (within your home network).
- Laptop knows:
  - Router’s **IP** (default gateway, e.g., `192.168.1.1`).
  - Uses **ARP (Address Resolution Protocol)** to find:
    - “What MAC address corresponds to IP 192.168.1.1?”
  - ARP reply: “Router MAC = `AA:BB:CC:DD:EE:FF`”
- Laptop sends an Ethernet frame:
  - Destination MAC: `AA:BB:CC:DD:EE:FF`
  - Source MAC: your laptop’s MAC

So:

- **MAC** → local delivery to the next hop on your LAN.  
- **IP** → logical addressing for end‑to‑end delivery across networks.

### 4.3 Scope difference: MAC vs IP

- MAC:
  - Visible only in your local network segment.
  - Not used for routing across the internet.
- IP:
  - Visible across the internet.
  - Used by routers everywhere to send data closer to destination.

Analogy:

- **MAC address**: your **face** in a room — people in the room recognize you by it, but people in other cities don’t see your face.
- **IP address**: your **house address** — used by postal services worldwide.

---

## 5. How Domain, IP, and MAC Work Together (High Level Flow)

Let’s connect them with a simple example:

> You open a browser and go to `https://example.com`.

1. **Domain name → IP (DNS)**
   - Browser sees `example.com`.
   - Uses **DNS** to find the IP, say `93.184.216.34`.

2. **Your machine & router (local network)**
   - Your device has private IP, e.g., `192.168.1.10`.
   - Router is `192.168.1.1`.
   - To send data out, your device sends packets to router’s IP (default gateway).
   - It uses **ARP** to map `192.168.1.1` → router’s MAC (e.g., `AA:BB:CC:DD:EE:FF`).
   - Link layer sends frames using:
     - Source MAC: your device’s MAC.
     - Destination MAC: router’s MAC.

3. **Router & the Internet**
   - Router replaces your private source IP (`192.168.1.10`) with its **public IP**.
   - Now IP packet looks like:
     - Source IP: your router’s public IP (e.g., `122.160.45.23`)
     - Destination IP: `93.184.216.34`
   - Router sends packet into ISP network.
   - Within each local link/hop, frame-level communication uses **MAC addresses** of neighboring devices.
   - Across hops, IP stays; MAC changes hop by hop.

4. **Destination server**
   - Packets reach the server with destination IP = `93.184.216.34`.
   - At the last hop in the data center network, ARP resolves the server’s IP to its MAC.
   - Link layer delivers packets to the server’s NIC via MAC.

So:

- **Domain name** is used only at the **very beginning** by DNS.
- **IP address** is used by every router along the path.
- **MAC addresses** are used between neighboring devices on each link (hop).

---

## 6. What Is Routing?

Now that we know what addresses are, we can answer:

> How does the network decide *which path* to send packets along, from one IP to another, possibly across the world?

That’s **routing**.

### 6.1 Definition

**Routing** is the process of:

- Determining the path that data packets take from source IP to destination IP.
- Forwarding packets from router to router until they reach the destination network.

Routers use **routing tables** and **routing protocols** to make these decisions.

### 6.2 Routers and routing tables

A **router** is a device with:

- Multiple network interfaces (ports).
- A **routing table** — a list of rules like:

  - “To reach network `203.0.113.0/24`, send to next hop at `198.51.100.1` via interface 2.”
  - “To reach network `192.0.2.0/24`, use interface 3.”
  - “Default route: send everything else to my ISP.”

When a packet arrives at a router:

1. Router reads the **destination IP**.
2. Looks up the **best matching route** in its routing table.
3. Forwards packet out of the appropriate interface towards the **next hop**.

Each router only knows **where to send the packet next**, not the entire world map.

### 6.3 Next hop concept

Packets move **hop‑by‑hop**:

- Your device → Home router (hop 1)
- Home router → ISP router (hop 2)
- ISP router → Regional router (hop 3)
- … many hops …
- Last ISP router → Destination server’s router (final hops)
- Router → Server

Each hop is just: “Send to the next router that is closer to the destination network.”

### 6.4 Static vs dynamic routing (high level)

- **Static routing**:
  - Routes manually configured by a network admin.
  - Simple, used in small networks.

- **Dynamic routing**:
  - Routers learn and update their routes using routing protocols.
  - Examples (just names for now):
    - **BGP** (Border Gateway Protocol) — between ISPs / large networks.
    - **OSPF, IS-IS** — within an organization or ISP’s internal network.

Dynamic routing allows:

- Automatic adaptation if a link fails.
- Always trying to find a workable path between two networks.

### 6.5 Default gateway

On your PC/phone, there’s a setting called **default gateway** (usually your router’s IP, like `192.168.1.1`):

- If your device wants to send a packet to an IP outside the local network:
  - It sends it to the **default gateway**.
  - The router then routes it towards the internet.

Think: **default gateway** = “If I don’t know where this destination is, ask that guy (the router).”

---

## 7. Visual Summary (Mental Picture)

Imagine this stacked view when you visit a website:

1. **You (Human)**
   - Type `https://myapp.com` in the browser.

2. **Domain Name**
   - Browser uses DNS to convert `myapp.com` → IP `203.0.113.5`.

3. **IP Level (Global)**
   - Packets contain:
     - Source IP: your router’s public IP (e.g., `122.160.45.23`)
     - Destination IP: `203.0.113.5`
   - Routers all over the world read destination IP and forward packets closer to `203.0.113.0/24`.

4. **MAC Level (Local per hop)**
   - On each link:
     - Frame includes source MAC & destination MAC for **just that hop**.
   - MAC addresses change at every router hop; IPs remain.

5. **Routing**
   - Each router:
     - Checks destination IP.
     - Consults routing table.
     - Chooses next hop.

6. **Server**
   - Final router resolves server IP → server MAC using ARP.
   - Delivers frame to server’s network card.

Throughout this process, different “addresses” are used at different scopes and layers.

---

## 8. How This Fits Your Phase 1 Roadmap

From your roadmap, in Phase 1 you’re learning:

- How the internet works  
- How computers communicate and send data  
- Domain Name, IP & MAC Addresses and Routing  
- How ISP and DNS work together to deliver data  

This tutorial covers the conceptual core of that bullet:

- **Domain name** → human‑friendly name → resolved via DNS to IP  
- **IP address** → global logical address for routing across networks  
- **MAC address** → hardware address for local link communication  
- **Routing** → process of moving packets from one IP network to another, hop‑by‑hop

Later topics (HTTP/HTTPS, hosting, browsers, backends) will all sit **on top of** this foundation.

---

If you want to go one step further, I can:

- Give you **practical commands** (`ping`, `nslookup`, `tracert`/`traceroute`, `arp -a`, `ipconfig`/`ifconfig`) to see real IPs, MACs, DNS, and routing from your own machine.
- Or provide a short quiz / flashcards to help lock in the differences between domain, IP, MAC, and routing.

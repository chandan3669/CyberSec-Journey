# 🌐 Networking Notes

---

## 🧱 1. OSI Model (Simple Breakdown)

The **OSI Model** is a 7-layer framework that explains how data travels across a network.  
Each layer has a specific role.

---

### 🔻 Layer 1 — Physical
- Handles **hardware transmission**
- Sends raw bits (**0s and 1s**)
- Includes: cables, signals, voltage, connectors

---

### 🔻 Layer 2 — Data Link
- Transfers data between **directly connected devices**
- Converts bits → **frames**
- Uses **MAC addresses**
- Performs **error detection**

---

### 🔻 Layer 3 — Network
- Handles **routing & logical addressing**
- Uses **IP addresses**
- Decides path from source → destination

---

### 🔻 Layer 4 — Transport
- Ensures **data delivery**
- Breaks data into **segments**
- Manages:
  - Flow control
  - Error handling
- Protocols:
  - TCP
  - UDP

---

### 🔻 Layer 5 — Session
- Manages **connections between applications**
- Functions:
  - Start session
  - Maintain session
  - End session

---

### 🔻 Layer 6 — Presentation
- Handles **data formatting**
- Functions:
  - Encryption 🔐
  - Compression 📦
  - Translation

---

### 🔻 Layer 7 — Application
- Closest to **end user**
- Provides services like:
  - Web browsing
  - Email
  - File transfer

---

## ⚔️ 2. TCP vs UDP

Both operate at the **Transport Layer**, but behave differently.

---

### 🟢 TCP (Transmission Control Protocol)

- Connection-oriented (3-way handshake)
- Reliable ✔️
- Ordered delivery ✔️
- Slower due to error checking

**Used in:**
- HTTP / HTTPS
- Email
- File transfer
- Banking systems

---

### 🔴 UDP (User Datagram Protocol)

- Connectionless
- Fast ⚡
- No guarantee of delivery ❌
- No ordering ❌

**Used in:**
- Video streaming
- Online gaming
- VoIP calls
- DNS

---

### 🧠 Quick Summary

> **TCP → Reliability**  
> **UDP → Speed**

---

## 🔌 3. Common Protocols & Ports

| Protocol | Port | Purpose |
|---------|------|--------|
| HTTP    | 80   | Web (unsecured) |
| HTTPS   | 443  | Secure web |
| FTP     | 21   | File transfer |
| SSH     | 22   | Secure remote access |
| Telnet  | 23   | Remote login (insecure) |
| SMTP    | 25   | Send email |
| DNS     | 53   | Domain resolution |
| DHCP    | 67/68| Auto IP assignment |
| POP3    | 110  | Receive email |
| IMAP    | 143  | Email sync |

---

## 🌍 4. How DNS Works (Step-by-Step)

Example: `kiit.ac.in`

---

### 🔄 DNS Resolution Flow

1. **Browser Cache**
   - Checks if IP already known

2. **OS Cache**
   - Checks system-level cache

3. **DNS Resolver**
   - Request sent to ISP resolver

4. **Root Server**
   - Points to TLD server (.com, .in)

5. **TLD Server**
   - Points to authoritative server

6. **Authoritative Server**
   - Returns correct IP address

7. **Response Returned**
   - IP sent back + cached

8. **Connection**
   - Browser connects to server using IP

---

## 🚀 Final Insight

- OSI → How networking is structured  
- TCP vs UDP → How data is delivered  
- Ports → Where services run  
- DNS → How domains become IPs  

> Master these = Strong networking foundation 🔥

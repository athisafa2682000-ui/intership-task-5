# 🧩 Task 5: Capture and Analyze Network Traffic Using Wireshark (Windows)

## 🎯 Objective
To capture live network packets and analyze different protocols (TCP, DNS, HTTP, and ARP) using **Wireshark** on a **Windows operating system**.

---

## 🛠️ Tools Used
- **Wireshark (Windows version)** – Free network packet analyzer  
- **Operating System:** Windows 10 / 11  
- **Network Interface:** Wi-Fi (active network connection)

---

## 📋 Steps Performed

1. **Installed Wireshark**
   - Downloaded and installed from the official site: [https://www.wireshark.org](https://www.wireshark.org)

2. **Opened Wireshark**
   - Launched the application and selected the **Wi-Fi** network interface to capture packets.

3. **Started Live Capture**
   - Clicked on the **blue shark fin icon** to begin live packet capture.

4. **Generated Network Traffic**
   - Browsed several websites to produce **HTTP** and **DNS** traffic.
   - Opened **Command Prompt** and ran:
     ```cmd
     ping google.com
     ```
     This generated **ICMP** packets for analysis.

5. **Stopped Capture**
   - Stopped packet capture after about one minute using the **red stop button**.

6. **Applied Protocol Filters**
   - Used the following display filters to analyze each protocol separately:
     - `tcp` – Transmission Control Protocol
     - `http` – Web browsing traffic
     - `dns` – Domain Name System traffic
     - `arp` – Address Resolution Protocol

7. **Saved the Capture**
   - Saved the capture file as **TCP_TASK5.pcapng** using **File → Save As**.

8. **Analyzed the Results**
   - Reviewed packet details (source, destination, protocol type, and payload).
   - Observed real-time communication between local and remote hosts.

---

## 🔍 Protocol Analysis

### **1. TCP (Transmission Control Protocol)**
- Provides reliable and ordered data delivery between devices.
- Observed **SYN**, **ACK**, and **FIN** flags during connection setup and termination.
- Example:
  - Source: 192.168.1.3 → Destination: 142.250.x.x  
  - Info: `TCP SYN → TCP connection established`

---

### **2. HTTP (Hypertext Transfer Protocol)**
- Used for communication between web clients and servers over port 80.
- Captured both **GET** and **POST** requests.
- Example:
  - Request: `GET /index.html HTTP/1.1`
  - Response: `HTTP/1.1 200 OK`

---

### **3. DNS (Domain Name System)**
- Converts domain names into IP addresses.
- Uses UDP on port 53.
- Example:
  - Query: `A google.com`
  - Response: `142.250.x.x`

---

### **4. ARP (Address Resolution Protocol)**
- Resolves IP addresses to MAC addresses within a LAN.
- Example:
  - Request: *Who has 192.168.1.5? Tell 192.168.1.3*  
  - Reply: *192.168.1.5 is at 00:1A:2B:3C:4D:5E*

---

## 📈 Findings

- Successfully captured and identified multiple protocols: **TCP**, **HTTP**, **DNS**, and **ARP**.
- Verified protocol behavior according to the **OSI model**:
  - TCP → Transport Layer  
  - HTTP, DNS → Application Layer  
  - ARP → Data Link Layer  
- Observed normal network communication patterns with no errors.

---

## 🧠 Key Learning Outcomes

- Learned to perform **live packet capture** and **filter specific traffic** using Wireshark on Windows.
- Understood the purpose and behavior of major network protocols.
- Gained hands-on experience in **network troubleshooting and protocol analysis**.

---

## 💾 Deliverables

- **Packet Capture File:** `TCP_TASK5.pcapng`  
- **Documentation File:** `README.md`

---

## 🧾 Conclusion
Task 5 was successfully completed on the **Windows operating system** using **Wireshark**.  
Captured and analyzed real-time packets for **TCP**, **HTTP**, **DNS**, and **ARP** protocols.  
The task provided practical exposure to network communication, packet structure, and Wireshark usage for **protocol-level analysis and troubleshooting**.

---

### 👩‍💻 Author
**Atheeka Bi Safa**  
**Project:** Network Security Lab – Task 5  
**Tool Used:** Wireshark (Windows)

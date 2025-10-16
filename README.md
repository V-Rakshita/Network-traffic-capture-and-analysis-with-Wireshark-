# Network-traffic-capture-and-analysis-with-Wireshark
## AIM:
To capture and analyze network traffic using Wireshark in order to observe protocols, packets, and potential anomalies.
## Requirements:
- **Hardware:**
    - Computer with internet access
    - Network adapter (Ethernet/Wi-Fi)
- **Software:**
    - Wireshark (latest stable version)
    - Sample PCAP files (optional for offline analysis)
## Architecture:
```mermaid
flowchart TD
    A[Network Interface Card] --> B[Wireshark Packet Capture Engine]
    B --> C[Packet Decoder & Protocol Analyzer]
    C --> D[Packet Display & Filtering Interface]
    D --> E[Investigator Analyzes Network Data]
    E --> F[Findings: IPs, Ports, Protocols, Anomalies]
```
## DESIGN STEPS:
### Step 1:
Install Wireshark on the system.

### Step 2:
Launch Wireshark and select the network interface (Ethernet/Wi-Fi).

### Step 3:
Start the capture, apply filters (like http, tcp, ip.addr == x.x.x.x) to analyze specific traffic, and stop the capture after observing relevant data.
### Step 4:
**Analyze traffic to identify:**
  - Source & Destination IP addresses
  - Protocols (HTTP, DNS, TCP, UDP, etc.)
  - Suspicious activities (e.g., unusual ports, repeated requests).


## OUTPUT:
<img width="979" height="397" alt="image" src="https://github.com/user-attachments/assets/37ecc8d1-ab66-4c47-bf60-e4eb379dd1c2" />

<img width="979" height="494" alt="image" src="https://github.com/user-attachments/assets/2575b41b-e86a-4e35-b8f7-a68b00dbf341" />

•	ip.src == 140.82.113.22

<img width="979" height="468" alt="image" src="https://github.com/user-attachments/assets/2399afc7-fec5-4962-a89d-35cc9e938b9e" />

•	tcp.port==80 (HTTP)

<img width="628" height="339" alt="image" src="https://github.com/user-attachments/assets/2570ac11-e945-4028-9517-d0ce75c423ca" />

•	udp.port==53 (DNS)

<img width="979" height="521" alt="image" src="https://github.com/user-attachments/assets/987d892d-aa1e-4b64-9649-f8a08ebeb9a7" />

<img width="979" height="531" alt="image" src="https://github.com/user-attachments/assets/9885b751-ae1a-4191-a7fe-6a6ce9a81215" />



## RESULT:
Network traffic was successfully captured and analyzed using Wireshark.

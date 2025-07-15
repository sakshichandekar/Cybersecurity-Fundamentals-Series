# 🌐 IP, TCP, UDP, and Ports

Understanding how devices communicate over a network is foundational in cybersecurity. Let’s break it down:

---

## 📌 IP Address

- A unique identifier assigned to each device on a network.
- Example: `192.168.1.10`
- **IPv4**: 32-bit address (e.g., `192.168.1.1`)
- **IPv6**: 128-bit address (e.g., `2001:0db8:85a3::8a2e:0370:7334`)
- **Public IP**: Used over the internet  
- **Private IP**: Used inside local networks (e.g., `192.168.x.x`)

---

## 🔁 TCP vs UDP

| Feature       | TCP (Transmission Control Protocol) | UDP (User Datagram Protocol) |
|---------------|-------------------------------------|------------------------------|
| Type          | Connection-oriented                 | Connectionless               |
| Reliability   | Reliable, ensures delivery          | Unreliable, no guarantee     |
| Speed         | Slower due to overhead              | Faster, lightweight          |
| Use Cases     | Web (HTTP/HTTPS), Email (SMTP)      | DNS, VoIP, Online gaming     |

---

## 🔢 What Are Ports?

- Think of ports like “doors” on a device for specific services.
- **Example**:  
   - Port **80** = HTTP (web traffic)  
   - Port **443** = HTTPS  
   - Port **22** = SSH

### Port Ranges:
- `0–1023`: Well-known ports (reserved)
- `1024–49151`: Registered ports
- `49152–65535`: Dynamic/private ports

---

## 🧰 Real-World Tip

Use these commands on your own system:
```bash
ip a              # Show your IP address (Linux)
netstat -tuln     # Show active TCP/UDP ports

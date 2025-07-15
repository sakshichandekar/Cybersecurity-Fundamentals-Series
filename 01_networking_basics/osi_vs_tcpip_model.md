# 🧬 OSI vs TCP/IP Model

Understanding how data travels over a network is essential in cybersecurity. These models explain the different **layers** involved in communication.

---

## 🌐 OSI Model (7 Layers)

| Layer | Name         | Function                                                                |
|-------|--------------|----------------------------------------------------------------------------------------|
| 7     | Application  | User-facing apps like web browsers, email clients (e.g., HTTP, FTP, SMTP)             |
| 6     | Presentation | Formats data so apps can understand it — encryption, compression, encoding            |
| 5     | Session      | Starts, maintains, and ends communication sessions between devices                    |
| 4     | Transport    | Breaks data into packets, adds port numbers, and ensures reliable delivery (TCP) or fast delivery (UDP) |
| 3     | Network      | Handles routing, IP addressing and finds the best path for data                         |
| 2     | Data Link    | Adds MAC address, ensures data is error-free between switches/routers                 |
| 1     | Physical     | Moves raw bits through cables, Wi-Fi, etc. actual hardware (e.g., Ethernet cables)  |


---

## 📦 TCP/IP Model (4 Layers)

| Layer | Name          | Corresponds To (OSI)            |
|-------|---------------|----------------------------------|
| 4     | Application   | OSI Layers 5–7                  |
| 3     | Transport     | OSI Layer 4                     |
| 2     | Internet      | OSI Layer 3                     |
| 1     | Network Access| OSI Layers 1–2                 |

---

## 🔍 Key Concepts:

- **Encapsulation**: Each layer adds its own header to data (like an onion 🧅)
- **Decapsulation**: At the receiver end, each layer removes its header
- OSI is a teaching model — TCP/IP is what’s actually used in real-world networking

---

## 🖼️ OSI vs TCP/IP – Visual Comparison

<p align="center">
  <img src="https://s8182.pcdn.co/wp-content/uploads/2014/06/063014_1912_TCPIPANDTHE1.jpg" alt="OSI vs TCP/IP Model Comparison" width="700"/>
</p>

> 📊 This diagram compares the OSI 7-layer model with the real-world TCP/IP model. Notice how some OSI layers are merged in TCP/IP!

---

## ✅ Summary:

- OSI = 7-layer conceptual model
- TCP/IP = 4-layer practical model used in real-world networks
- Knowing the layers is key to troubleshooting, hacking, and defending systems

---


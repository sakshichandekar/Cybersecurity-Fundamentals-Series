# 📡 Common Network Protocols:

Protocols define **how data is exchanged** over a network. In cybersecurity, knowing these is crucial because attackers often exploit them.

---

## 📌 Protocols Cheat Sheet

| Protocol | Full Form                  | Port | Purpose                                 | Secure? |
|----------|----------------------------|------|-----------------------------------------|---------|
| HTTP     | HyperText Transfer Protocol| 80   | Web browsing (insecure websites)        | ❌      |
| HTTPS    | HTTP Secure                | 443  | Encrypted web browsing (secure sites)   | ✅      |
| FTP      | File Transfer Protocol     | 21   | Transfer files over a network           | ❌      |
| FTPS     | FTP Secure                 | 990  | FTP with TLS encryption                 | ✅      |
| SFTP     | SSH File Transfer Protocol | 22   | Encrypted file transfer over SSH        | ✅      |
| SSH      | Secure Shell               | 22   | Remote login to servers (CLI access)    | ✅      |
| Telnet   | --                         | 23   | Remote login (insecure)                 | ❌      |
| SMTP     | Simple Mail Transfer Prot. | 25   | Sends email (outgoing)                  | ❌      |
| SMTPS    | SMTP Secure                | 465  | Sends email securely                    | ✅      |
| POP3     | Post Office Protocol v3    | 110  | Downloads emails to local client        | ❌      |
| POP3S    | POP3 Secure                | 995  | Secure version of POP3                  | ✅      |
| IMAP     | Internet Message Access    | 143  | Syncs email (keeps on server)           | ❌      |
| IMAPS    | IMAP Secure                | 993  | Secure version of IMAP                  | ✅      |
| DNS      | Domain Name System         | 53   | Resolves domain names to IPs            | ⚠️      |
| DHCP     | Dynamic Host Config Prot.  | 67/68| Assigns IPs automatically               | ⚠️      |
| SNMP     | Simple Network Mgmt Prot.  | 161  | Monitor/manage devices in a network     | ⚠️      |

> ℹ️ POP3 and IMAP are used by email clients to fetch emails. They're older protocols, and **often replaced by secure versions (POP3S, IMAPS)** or APIs in modern systems.

---

## 🔐 Why Cyber Pros Care About Protocols

### 🧠 Because protocols = attack surfaces.

- **HTTP / Telnet / FTP** transmit data in **plain text** — attackers can **sniff passwords**
- **SMTP** can be **spoofed** → phishing attacks
- **DNS** can be **poisoned**
- **SSH** can be brute-forced if misconfigured
- **SNMP** often runs with default settings → info leakage

---

## 🧨 Examples of Attacks

| Protocol | Possible Attack                                  |
|----------|--------------------------------------------------|
| HTTP     | Packet sniffing (e.g., Wireshark shows passwords)|
| FTP      | Credential harvesting                            |
| DNS      | DNS spoofing / redirection                       |
| SMTP     | Email spoofing / spam relay                      |
| Telnet   | Session hijacking                                |
| SNMP     | Network discovery / info leakage                 |

---

## 💡 Pro Tips

- ✅ Use **HTTPS** or **SFTP** instead of **HTTP** or **FTP**
- ❌ Don’t use **Telnet** or **FTP** in real environments — they send data without encryption
- 🔐 Learn how to recognize common ports like 22 (SSH), 80 (HTTP), 443 (HTTPS)
- 🔍 Watch out for unknown open ports — they can be a sign of malware or backdoors

> These habits make you think like a hacker **and** a defender.

---



# 🛡️ Cybersecurity Homelab  
#### By Yousef Ibrahim

This homelab is a virtualized network for practicing offensive and defensive cybersecurity techniques. It's built with multiple VMs, including a vulnerable web app, logging tools, and attacker environments — all designed to simulate real-world attack surfaces and monitoring workflows.

---

## 🖥️ Lab Architecture

- **Attacker Machine:** Kali Linux (Tools: Metasploit, Nmap, Burp Suite, John the Ripper)
- **Target Machine:** Metasploitable2 (vulnerable Linux image)
- **Web App:** DVWA (Damn Vulnerable Web App) on Debian
- **Logging/Monitoring:** Graylog stack with OpenSearch, MongoDB, and GELF input

---

## 🧰 Tools and Services

| Tool               | Purpose                                 |
|--------------------|-----------------------------------------|
| **Kali Linux**      | Penetration testing + offensive tools   |
| **Metasploitable**  | Vulnerable target for exploitation      |
| **DVWA**            | Web app to test web-based attacks       |
| **Graylog**         | Centralized log collection & monitoring |
| **Apache2/MariaDB** | DVWA backend stack                      |
| **Docker Compose**  | For managing Graylog stack              |

---

## 🌐 Network Diagram

📌 [Network Map](https://github.com/Yousefibrahim1/cybersecurity-homelab/blob/main/Screenshots/Network%20Map.png)

---

## 📂 Folder Structure

```
cybersecurity-homelab/
├── README.md
├── DVWA-Setup/
│   └── install-dvwa.sh
├── Graylog/
│   └── docker-compose.yml
├── Screenshots/
│   ├── dvwa-login.png
│   └── graylog-dashboard.png
└── Notes/
    └── tryhackme-writeups.md
```

---

## ⚡ Usage

1. **Clone the repo:**
```
git clone https://github.com/yousefibrahim/cybersecurity-homelab.git
```
2. Launch the Graylog stack:
```
cd Graylog
docker-compose up -d
```
3. Access DVWA:
```
Open your browser and visit: http://192.168.56.105/dvwa

Default credentials:
Username: admin
Password: password
```

## 🧠 What I'm Learning
- Network enumeration, scanning, and web exploitation

- Configuring and securing logging pipelines

- Vulnerability assessment using Metasploit and manual tools

- Real-time event logging with Graylog and GELF inputs

## 🎯 TryHackMe Modules Completed
Cyber Defense Frameworks

- Cryptography

- Compromising Active Directory

- Endpoint Security Monitoring

- Network Security

- Metasploit

- Splunk 1 & 2


## 🧠 About This Project
This homelab is part of my self-directed learning in cybersecurity while studying at Marist University. I'm actively expanding the setup and documenting my process as I go. Always open to feedback or ideas — feel free to reach out!

## 📜 License
MIT — feel free to fork, adapt, or build upon it ✌️

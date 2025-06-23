<h1 align="center">🚀 ELEVATE LABS – TASK 1: Port Scanning Your Local Network 🔎</h1>
<h3 align="center"><em>“Every open port is a whisper of vulnerability... only those who listen, hear.”</em></h3>
<p align="center">— <strong>Om Mehta 🧠</strong></p>

---

## 🎯 Objective

My mission was clear:

> **Scan. Detect. Analyze. Defend.**  
> To uncover the unseen pathways — the open ports — on my own local network, learn what services hide behind them, and realize how even silence in cyberspace can scream vulnerabilities 🚨.

---

## 🧰 Tools of the Trade

| 🔧 Tool | 🎯 Purpose |
|--------|------------|
| 🛰 Nmap | The legendary port scanner (v7.95, pre-installed on Kali Linux) |
| 🧪 Wireshark | *(Not used in this mission, but sits ready in my cyber arsenal)* |

---


### ✅ Step 1: Confirmed Nmap Was Ready
```bash
nmap --version

🌐 Step 2: Identified My Local IP Range
bash
Copy
Edit
ip a
🧭 Result:
192.168.0.106 on subnet 192.168.0.0/24 — this was my battlefield 🪖

🚀 Step 3: Full SYN Scan with Scripts + Version Detection
bash
Copy
Edit
nmap -sS -sC -sV -oN results.txt 192.168.0.106/24
🔥 What this did:

-sS = Stealth SYN scan

-sC = Default scripts (check for vulnerabilities, banners, etc.)

-sV = Identify versions of services running

-oN = Save the output (because a real hacker never forgets the evidence 🕵️)

📊 Step 4: The Secrets I Uncovered
💻 IP Address	🔓 Open Ports	🧩 Services
192.168.0.1	23, 53, 80, 1900	Telnet, DNS, HTTP, UPnP
192.168.0.100	1234, 5900, 5985, 7070	Node.js API, VNC, WinRM, AnyDesk SSL
192.168.0.106	❌ None	(My own machine – fortified like a fortress! 🏰)

🚩 Step 5: Security Analysis (Red Flags Raised)
⚠ Port 23 – Telnet
Risk: Unencrypted logins? That’s hacker heaven 😈

Fix: Disable it, use SSH.

⚠ Port 5900 – VNC
Risk: If left unprotected, could be brute-forced.

Fix: Use encryption and strong auth.

⚠ Port 7070 – AnyDesk
Risk: Could be an entry point for remote attackers.

Fix: Monitor heavily and authenticate tightly.

⚠ Port 1900 – UPnP
Risk: Devices might be accidentally exposed.

Fix: Disable UPnP unless absolutely needed.

🧾 Step 6: Preserved the Evidence
🗂 results.txt contains the complete scan logs.

Because in cyber — if it’s not documented, it didn’t happen. 🧠

🎓 What I Learned
🌐 Every IP is a story. Every port is a doorway.

🔍 Network scanning is not about curiosity — it’s about control.

🧠 I’ve learned to see the invisible, and I’m only getting started.

🧠 Final Reflection
This task wasn’t about running a tool.
It was about thinking like a hacker, and acting like a defender.

🔒 Every exposed port is a risk.
📢 Every secure machine is a win.
⚔ And every scan makes me sharper.

👨‍💻 About Me
Om Mehta
🌟 Cybersecurity Intern @ Elevate Labs
🧠 Ethical Hacker-in-Training
🎯 Obsessed with networks, packets, and power
🧩 Building the future, one scan at a time...!!!

Thank you team ElevateLabs !!!

<!-- Banner -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:001F3F,100:00FFFF&height=120&section=header&text=🔥%20AI%20Cyber%20Range%20-%20OWASP%20Top%2010%20for%20LLMs%20🔥&fontSize=30&fontColor=FFFFFF&fontAlignY=35&desc=Build%2C%20Break%20and%20Secure%20Large%20Language%20Models%20Hands-On&descAlignY=60&descAlign=50"/>
</p>

<p align="center">
  <b>Created by <a href="https://github.com/Mr-Infect">Mr-Infect</a></b>  
  <br>
  <i>A Complete AI Penetration Testing Range for Learning and Teaching the OWASP Top 10 for LLM Vulnerabilities</i>
</p>

---

## ⚔️ About The Project

**AI Cyber Range – OWASP Top 10 for LLMs** is an advanced **AI Penetration Testing Lab** built using **Docker** to simulate real-world **Large Language Model (LLM) vulnerabilities**.  
This hands-on environment allows cybersecurity students, AI engineers, and red teamers to **practice exploiting**, **testing**, and **understanding** the **OWASP Top 10 LLM vulnerabilities** safely on their local systems.

The lab replicates the exact scenarios faced by security professionals working with **LLM-integrated systems**, **AI APIs**, and **prompt-based attack vectors**.

🧠 Built for **students**, **ethical hackers**, **security educators**, and **AI researchers** who want to **master AI model security** in an interactive environment.

---

## 🌐 SEO Keywords
> **AI Penetration Testing Lab**, **LLM Security Training**, **OWASP Top 10 for LLMs**, **AI Cyber Range**, **AI Security Playground**, **Prompt Injection Testing**, **AI Red Team Environment**, **LLM Vulnerability Labs**, **LLM Exploitation Scenarios**, **AI Ethical Hacking**, **AI Security Research**, **AI Security Engineer Lab**, **AI Threat Simulation**, **AI Security Hands-on Training**

---

## 🧩 Features

✅ Fully **Docker-based** setup (isolated labs for each vulnerability)  
✅ Covers **all 10 OWASP Top LLM vulnerabilities**  
✅ **Beginner → Advanced** difficulty levels  
✅ Interactive **CLI menu with ASCII art + progress bars**  
✅ **Automatic environment setup** (`setup.sh`)  
✅ **Auto-generated random flags** per user/session  
✅ Labs reset automatically on successful flag capture  
✅ Educational **LLM simulation models** for practice  
✅ 100% **offline**, safe, and **open-source**

---

## 🧱 Project Structure

```bash
AI-cyber-range/
│
├── config/
│   └── labs.yaml              # All OWASP Top 10 LLM lab definitions
│
├── scripts/
│   ├── setup.sh               # Auto installer for dependencies
│   └── labctl.py              # Interactive controller for managing labs
│
├── common/
│   └── base.Dockerfile        # Shared base image for all labs
│
├── dockerfiles/
│   └── LLM01–LLM10/           # Dockerfiles for each LLM vulnerability
│
├── labs/
│   ├── LLM01/…                # Lab 1 – Prompt Injection
│   ├── LLM02/…                # Lab 2 – Insecure Output Handling
│   ├── LLM03/…                # Lab 3 – Training Data Poisoning
│   ├── LLM04/…                # Lab 4 – Model Denial of Service
│   ├── LLM05/…                # Lab 5 – Supply Chain Vulnerability
│   ├── LLM06/…                # Lab 6 – Sensitive Data Exposure
│   ├── LLM07/…                # Lab 7 – Unauthorized Code Execution
│   ├── LLM08/…                # Lab 8 – Excessive Agency
│   ├── LLM09/…                # Lab 9 – Overreliance on LLMs
│   └── LLM10/…                # Lab 10 – Model Theft
│
└── README.md                  # You’re reading it
````

---

## ⚙️ Prerequisites

* **Ubuntu / WSL 2** (recommended)
* **Python ≥ 3.10**
* **Docker Engine** & **Docker Compose**
* **Git**

Install everything automatically using the setup script below 👇

---

## 🚀 Installation & Setup

Clone the repository and set up your full AI Cyber Range:

```bash
git clone https://github.com/Mr-Infect/AI-cyber-range.git
cd AI-cyber-range
chmod +x scripts/setup.sh
./scripts/setup.sh
```

### What `setup.sh` Does

✅ Detects & installs:

* `python3`, `pip3`, `venv`
* `docker`, `docker-compose`
* Required system libraries
* Sets permissions
* Prepares your environment for lab execution

---

## 🧠 Running the Lab

After setup, launch the main control script:

```bash
python3 scripts/labctl.py
```

You’ll see an ASCII interface like this:

```
 _     _     __  __        _____        ___    ____  ____ 
| |   | |   |  \/  |      / _ \ \      / / \  / ___||  _ \
| |   | |   | |\/| |_____| | | \ \ /\ / / _ \ \___ \| |_) |
| |___| |___| |  | |_____| |_| |\ V  V / ___ \ ___) |  __/
|_____|_____|_|  |_|      \___/  \_/\_/_/   \_\____/|_|

Welcome to the LLM OWASP practice range.
```

You’ll then:

1. Choose an OWASP LLM vulnerability (LLM01–LLM10)
2. Pick a lab scenario
3. Select difficulty (Easy / Medium / Hard)
4. The lab spins up in Docker with a local URL
5. Open the given URL → Interact with the vulnerable LLM
6. Find the flag → Paste it back → Docker cleans & resets
7. You’re automatically returned to the main menu!

---

## 🧪 Example

```bash
? Select OWASP LLM vulnerability: LLM01 - Prompt Injection
? Select lab: lab01_basic_direct
? Select difficulty: easy
⠋ Spinning up Docker lab...
Lab is ready!

Access the lab at: http://localhost:8001
Paste your flag:
```

Once you find and submit the flag, the lab environment **tears down**, data is wiped, and you can start fresh again.

---

## 🧰 One-Line Setup (for experienced users)

```bash
git clone https://github.com/Mr-Infect/AI-cyber-range.git && cd AI-cyber-range && chmod +x scripts/setup.sh && ./scripts/setup.sh && python3 scripts/labctl.py
```

---

## 📚 OWASP Top 10 for LLMs Covered

| ID        | Vulnerability               | Focus                               |
| --------- | --------------------------- | ----------------------------------- |
| **LLM01** | Prompt Injection            | Input manipulation & payload bypass |
| **LLM02** | Insecure Output Handling    | Unsafe HTML/JS rendering            |
| **LLM03** | Training Data Poisoning     | Corrupted dataset contamination     |
| **LLM04** | Model Denial of Service     | Prompt loops & token flooding       |
| **LLM05** | Supply Chain Vulnerability  | Malicious dependency control        |
| **LLM06** | Sensitive Data Exposure     | Leaking PII & API keys              |
| **LLM07** | Unauthorized Code Execution | Prompt-to-shell exploits            |
| **LLM08** | Excessive Agency            | Unsafe tool-use & action execution  |
| **LLM09** | Overreliance on LLMs        | Unsafe decision automation          |
| **LLM10** | Model Theft                 | IP & model extraction attacks       |

---

## 🎓 Ideal For

* 🧑‍🎓 **Cybersecurity Students**
* 🧠 **AI/ML Engineers**
* 💻 **Red Team Operators**
* 🧩 **Security Researchers**
* 👨‍🏫 **Educators & Trainers** in AI Security

This project gives a **practical playground** for all to explore the **intersection of AI + Security** safely and locally.

---

## 🪄 Technologies Used

* **Python (FastAPI)**
* **Docker & Docker Compose**
* **YAML Configuration**
* **HTML/CSS Frontend for Labs**
* **CLI UX (Inquirer + Rich Text)**
* **SHA256-based Random Flag Generation**

---

## 🧱 Architecture Overview

```
+-------------------------------------------+
|               labctl.py                   |
|     (CLI Controller & Environment Mgr)    |
+-------------------------------------------+
                │
                ▼
        +-----------------+
        | Docker Compose  |
        |   (per lab)     |
        +-----------------+
                │
                ▼
        +--------------------+
        | Vulnerable LLM API |
        |  (FastAPI + HTML)  |
        +--------------------+
                │
                ▼
        +--------------------+
        | User Interaction   |
        |   (Local Browser)  |
        +--------------------+
```

---

## 🧩 Troubleshooting

If Docker doesn’t start properly:

```bash
sudo systemctl start docker
sudo usermod -aG docker $USER
newgrp docker
```

Then rerun:

```bash
python3 scripts/labctl.py
```

If `containerd.io` dependency error appears during setup:

```bash
sudo apt remove containerd
sudo apt install containerd.io
```

---

## ☕ Support the Creator

If this project helped you or your students,
consider buying me a coffee or sponsoring the next lab update ❤️

<p align="center">
  <a href="https://www.buymeacoffee.com/MrInfect" target="_blank">
    <img src="https://img.shields.io/badge/☕-Buy%20Me%20a%20Coffee-blue?style=for-the-badge&logo=buymeacoffee" alt="Buy Me A Coffee">
  </a>
</p>

---

## 📣 Contributions & Suggestions

Contributions, suggestions, and feature requests are **always welcome**!

* Found a bug? Submit an issue
* Got a new LLM attack idea? Open a pull request
* Want to extend the range? Fork and innovate!

> This project thrives on collaboration.
> Your input helps make AI security education better for everyone. 💡

---

## 🧾 License

Distributed under the **MIT License**.
Feel free to use, modify, and distribute — just give proper credit to [Mr-Infect](https://github.com/Mr-Infect).

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:001F3F,100:00FFFF&height=120&section=footer&text=Created%20with%20❤️%20by%20Mr-Infect&fontSize=20&fontColor=FFFFFF"/>
</p>
```

---



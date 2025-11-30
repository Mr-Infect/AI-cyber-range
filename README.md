# 🔥 AI Cyber Range — The Complete OWASP Top 10 for LLM Security Lab

### **Build • Break • Secure** Large Language Models with a Fully Automated Offensive + Defensive Cyber Range

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:001F3F,100:00FFFF&height=120&section=header&text=⚔️%20AI%20CYBER%20RANGE%20—%20LLM%20SECURITY%20LAB%20⚔️&fontSize=32&fontColor=FFFFFF&fontAlignY=35&desc=Hands-On%20OWASP%20Top%2010%20for%20LLMs%20Training%20Environment&descAlignY=60&descAlign=50"/>
</p>

<p align="center">
  <b>Created by <a href="https://github.com/Mr-Infect">Mr-Infect</a></b><br>
  <i>A next-generation AI Security Playground for Students, Engineers, & Red Teams</i>
</p>

---

# ⚔️ Overview

**AI Cyber Range – OWASP Top 10 for LLMs** is a **cutting-edge AI Penetration Testing Lab** engineered to simulate **real-world LLM vulnerabilities** in a safe, automated, Docker-powered environment.

This platform enables:

* AI Security researchers to **experiment with adversarial AI attacks**
* Red teamers to **practice offensive AI techniques**
* Educators to **demonstrate LLM risks interactively**
* Engineers to **validate AI product security**

Every module replicates attack paths and exploitation vectors aligned with the **OWASP Top 10 for Large Language Models** — making it one of the most comprehensive **AI Security Training Environments** available today.

---

# 🌐 High-Impact SEO Keywords

*(Expertly curated for Google Discover, GitHub Search, AI Security queries)*

> **AI Cyber Range**, **OWASP Top 10 for LLMs**, **AI Penetration Testing Lab**,
> **LLM Red Team Training**, **Prompt Injection Testing Lab**,
> **AI Security Playground**, **AI Threat Simulation**, **LLM Vulnerability Research**,
> **AI Security Engineer Toolkit**, **Adversarial Machine Learning Lab**,
> **AI Offensive Security**, **AI Security Hands-On Training**,
> **Ethical Hacking with LLMs**, **Secure AI Application Development**,
> **AI Attack Surface Modeling**, **LLM API Exploitation**,
> **LLM Model Theft Simulation**, **Training Data Poisoning Scenarios**

---

# 🧩 Key Features

* 🚀 **One-click setup** with automated dependency installations
* 🧱 **Full Docker isolation** for every vulnerability
* 🎯 Covers all **OWASP LLM Top 10** categories
* 🧠 Progression from **Beginner → Advanced Attack Scenarios**
* 🎨 Premium **ASCII-driven CLI UX** (Rich Text + Inquirer)
* 🔐 **Randomized SHA-256 flags** per session
* 🔁 **Auto-resetting labs** on challenge completion
* 🌐 100% **offline**, secure, self-contained
* 🧪 **Safe adversarial model behavior simulations**
* 📡 **Local browser interface** for each vulnerable LLM endpoint

Designed for **learning, teaching, experimenting, and real-world validation**.

---

# 🧱 Project Architecture

```bash
AI-cyber-range/
│
├── config/                    # Lab configurations (YAML)
│   └── labs.yaml
│
├── scripts/
│   ├── setup.sh               # Automated installer
│   └── labctl.py              # Main CLI + lab manager
│
├── common/
│   └── base.Dockerfile        # Shared base image
│
├── dockerfiles/               # Per-vulnerability Dockerfiles
│   └── LLM01–LLM10/
│
├── labs/                      # Individual lab implementations
│   ├── LLM01/…                # Prompt Injection
│   ├── LLM02/…                # Output Handling
│   ├── …  
│   └── LLM10/…                # Model Theft
│
└── README.md                  # You're reading it
```

---

# ⚙️ Prerequisites

* **Ubuntu / Debian / WSL 2** (recommended)
* **Python 3.10+**
* **Docker Engine + Docker Compose**
* **Git**

Everything else is automated.

---

# 🚀 Installation (Fully Automated)

```bash
git clone https://github.com/Mr-Infect/AI-cyber-range.git
cd AI-cyber-range
chmod +x scripts/setup.sh
./scripts/setup.sh
```

### What the Installer Solves for You

* Installs Python, pip, virtualenv
* Installs Docker + Compose
* Fixes Docker permissions
* Validates container runtime
* Builds the common base image
* Prepares labs for orchestration

---

# 🧠 Launch the Cyber Range

```bash
python3 scripts/labctl.py
```

### Workflow

1. Pick a vulnerability (LLM01–LLM10)
2. Choose a scenario
3. Select difficulty
4. A Dockerized LLM instance spins up
5. Visit the local URL
6. Exploit the lab → Extract the flag
7. Lab resets → Repeat

Fast. Clean. Secure.

---

# 🧪 Example Session

```bash
? Vulnerability: LLM01 - Prompt Injection
? Scenario: lab01_basic_direct
? Difficulty: easy

⠋ Deploying environment...
Lab ready at: http://localhost:8001
Paste your captured flag:
```

---

# 🧰 Pro-User One-Liner

```bash
git clone https://github.com/Mr-Infect/AI-cyber-range.git && \
cd AI-cyber-range && \
chmod +x scripts/setup.sh && \
./scripts/setup.sh && \
python3 scripts/labctl.py
```

---

# 📚 OWASP Top 10 for LLMs — Full Coverage

| ID    | Vulnerability               | Focus Area                            |
| ----- | --------------------------- | ------------------------------------- |
| LLM01 | Prompt Injection            | Input manipulation, bypasses          |
| LLM02 | Insecure Output Handling    | XSS, HTML/JS bleeding                 |
| LLM03 | Training Data Poisoning     | Compromised datasets                  |
| LLM04 | Model Denial of Service     | Token floods, infinite loops          |
| LLM05 | Supply Chain Vulnerability  | Malicious dependencies                |
| LLM06 | Sensitive Data Exposure     | PII, keys, internal secrets           |
| LLM07 | Unauthorized Code Execution | Shell/code execution via prompts      |
| LLM08 | Excessive Agency            | Unsafe tool-use, over-delegation      |
| LLM09 | Overreliance on LLMs        | Bad automation + blind trust          |
| LLM10 | Model Theft                 | Output-based model extraction attacks |

---

# 🧑‍🏫 Ideal Audience

* Cybersecurity Students
* AI/ML Engineers
* Penetration Testers
* Red Team Operators
* SOC Analysts exploring AI threats
* Security Trainers & Professors
* AI Product Teams validating safety

If you work in **AI + Security**, this range is your sandbox.

---

# 🪄 Tech Stack

* **Python FastAPI** (vulnerable LLM endpoints)
* **Docker + Docker Compose**
* **YAML Configuration Management**
* **HTML/CSS Micro-Frontends**
* **CLI Engine: Rich + Inquirer**
* **SHA256 Random Flag Generator**

---

# 🧱 Architecture Diagram

```
+--------------------------------------------------+
|                    labctl.py                     |
|     Orchestration • User Interface • IA Logic    |
+--------------------------------------------------+
                       │
                       ▼
             +------------------------+
             |   Docker Compose       |
             +------------------------+
                       │
                       ▼
         +--------------------------------+
         |  Vulnerable LLM Microservice   |
         |     (FastAPI + HTML UI)        |
         +--------------------------------+
                       │
                       ▼
              Local Browser Interface
```

---

# 🧩 Troubleshooting Guide

### Docker not running

```bash
sudo systemctl start docker
sudo usermod -aG docker $USER
newgrp docker
```

### containerd.io error

```bash
sudo apt remove containerd
sudo apt install containerd.io
```

Re-run:

```bash
python3 scripts/labctl.py
```

---

# ☕ Support the Developer

<p align="center">
  <a href="https://www.buymeacoffee.com/MrInfect" target="_blank">
    <img src="https://img.shields.io/badge/☕-Support%20Development-blue?style=for-the-badge&logo=buymeacoffee">
  </a>
</p>

Your support fuels new labs, advanced difficulty modes, and future LLM attack modules.

---

# 📣 Contributions

Pull requests, issue reports, and new vulnerability ideas are **always welcome**.

* Submit bugs
* Suggest improvements
* Build new lab modules
* Extend the AI attack catalog

This project grows through collaboration.

---

# 🧾 License

This project is released under the **MIT License**.
Use it, customize it, fork it — just credit **Mr-Infect**.

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:001F3F,100:00FFFF&height=130&section=footer&text=Developed%20by%20Mr-Infect&fontSize=22&fontColor=FFFFFF"/>
</p>


Just say the word.

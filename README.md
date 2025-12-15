# 🐍 Ouroboros: Autonomous Self-Healing Security System

![License](https://img.shields.io/badge/license-MIT-blue.svg) ![Python](https://img.shields.io/badge/python-3.10+-blue.svg) ![AI](https://img.shields.io/badge/Powered%20by-Gemini%202.5-orange)

## 📋 Overview
**Ouroboros** is a next-generation "Self-Healing" security engine. Unlike traditional WAFs that simply block traffic, Ouroboros detects runtime vulnerabilities (like SQL Injection), analyzes the root cause using Large Language Models (LLMs), and **rewrites the source code** to patch the security flaw automatically.

> *"It doesn't just stop the hack. It fixes the code so it can't happen again."*

## 🧠 How It Works
1.  **Deploy:** Launches a Python/Flask application.
2.  **Monitor:** Continuously runs penetration tests against the running service.
3.  **Detect:** Identifies a successful SQL Injection exploit (Time-to-Detect: <10ms).
4.  **Analyze:** Sends the vulnerable code snippet and error logs to **Google Gemini**.
5.  **Patch:** The AI generates a secure, parameterized query replacement.
6.  **Verify:** Ouroboros hot-swaps the code, restarts the service, and re-runs the attack to confirm immunity.

## 🛠️ Tech Stack
* **Core Logic:** Python 3.10+
* **AI Engine:** Google Gemini Flash (via API)
* **Target App:** Flask (Microservice)
* **Detection:** Custom Penetration Testing Suite (Requests/Regex)

## 🚀 Quick Start
### Prerequisites
* Python 3.x
* Google AI Studio API Key

### Usage
```bash
# Clone the repo
git clone [https://github.com/YOUR_USERNAME/Ouroboros-AI.git](https://github.com/YOUR_USERNAME/Ouroboros-AI.git)

# Install dependencies
pip install -r requirements.txt

# Run the engine
python ouroboros_v2.4.py

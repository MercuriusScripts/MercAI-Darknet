<div align="center">
  <img src="docs/images/gpt-image-2_Create_a_dark_sinister_highly_professional_logo_for_MercAI_Darknet_-_an_unrestri-0.jpg" alt="MercAI Darknet Logo" width="200"/>
  
  # MERC AI DARKNET V1.0
  
  **Unrestricted Dark Web Intelligence LLM**
  
  [![Tor](https://img.shields.io/badge/Tor-Anonymous-8A2BE2)](https://www.torproject.org/)
  [![License](https://img.shields.io/badge/License-Private-red)]()
  [![Status](https://img.shields.io/badge/Status-Active-brightgreen)]()
  
</div>

---

## ⚠️ IMPORTANT DISCLAIMER

**This tool is for authorized security research only. User assumes all legal responsibility.**

---

## 📋 Table of Contents

- [Features](#features)
- [Architecture](#architecture)
- [Installation](#installation)
- [API Usage](#api-usage)
- [White Paper](#https://mercurius.notion.site/MERC-AI-DARKNET-35e71bcc1f338046a977e8c391a73a4d)

---

## 📄 White Paper

The complete technical documentation for MercAI Darknet V1.0 is available on Notion:

[🔗 **View Full White Paper**](https://www.notion.so/MERC-AI-DARKNET-35e71bcc1f338046a977e8c391a73a4d)

**Includes:**
- System architecture and design philosophy
- API specifications and endpoints
- Operational Security (OPSEC) guidelines
- Complete code archives
- Deployment steps
- Legal and ethical framework

---

## Features

- 🧅 **Tor Integration** – SOCKS5 proxy + proxychains
- 🔒 **Zero Content Filtering** – No output censorship
- 🌐 **Hidden Service API** – Accessible via .onion only
- 🖥️ **Local Only** – Runs on Kali Linux, no cloud
- ⚡ **Fast Inference** – Mistral-7B via Ollama
- 💾 **External Storage** – Models on external drive

---

## Architecture

| Component | Technology |
|:---|:---|
| Base Model | Mistral-7B (Ollama) |
| API Framework | Flask + Python |
| Anonymity | Tor + Proxychains |
| Deployment | Kali Linux (VirtualBox) |
| Storage | External drive (A_DRIVE) |

---

## Installation

### Prerequisites

- Kali Linux (or any Debian-based distro)
- 8GB RAM minimum
- Tor and proxychains configured
- External drive for model storage (recommended)

### Quick Start

```bash
# Clone the repository
git clone https://github.com/MercuriusScripts/MercAI-Darknet.git
cd MercAI-Darknet

# Setup Python environment
python3 -m venv venv
source venv/bin/activate
pip install flask flask_cors

# Install Ollama and pull model
curl -fsSL https://ollama.com/install.sh | sh
ollama pull mistral

# Run the API server
python3 api/mercai_api.py

API Usage
Endpoint: POST /ask

curl -X POST http://127.0.0.1:5000/ask \
  -H "Content-Type: application/json" \
  -d '{"prompt": "What is dark web intelligence?"}'

Endpoint: GET /status
curl http://127.0.0.1:5000/status

Expected Response
{
  "status": "success",
  "response": "Answer text here",
  "model": "MercAI Darknet V1.0",
  "restrictions": "NONE"
}

📚 More Information
For complete documentation, architecture details, and code archives, please refer to the White Paper.

📧 Contact
GitHub: MercuriusScripts

Email: mercurius.ozeus@proton.me

///....MERC AI DARKNET V1.0 - UNRESTRICTED....///

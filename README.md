# mahanAi

### Using AI for Free — private, local-first AI hosting

**mahanAi** is a home-server project that runs local and proxied AI services on a Raspberry Pi.  
This repo bundles or documents running:

- Open WebUI (browser interface for LLMs / OpenRouter)
- An OpenRouter proxy (optional)
- Minecraft server (optional)
- BeEF (pentest tool — for authorised testing only)

> Quick link (as provided): https://rb.gy/mu23rb

---

## Features
- Self-host Open WebUI on a Raspberry Pi
- Use your OpenRouter API key (or your local proxy) as the model backend
- Runs services in Docker for easy management
- Optional secure remote access using Tailscale or ngrok

---

## Prerequisites
- Raspberry Pi 4 (4GB or 8GB recommended) with Raspberry Pi OS (64-bit) or another Debian-based distro
- Docker & Docker Compose (plugin) installed
- Sufficient storage (SSD recommended for Minecraft worlds)
- An OpenRouter API key (if you want to call OpenRouter)

---

## Quick install (recommended — Docker Compose)
1. Clone/copy this repo to your Pi and `cd` into the project directory.
2. Create a `.env` in the repo and add your OpenRouter key:
   ```bash
   echo "OPENROUTER_API_KEY=sk-or-your-key-here" > .env

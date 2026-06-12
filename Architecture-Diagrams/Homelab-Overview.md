
# Homelab Overview

## Purpose

This homelab is designed to provide hands-on experience with systems engineering, AI infrastructure, virtualization, networking, automation, and self-hosted services.

The environment serves as both a learning platform and a production environment for the Jarvis AI Assistant project.

---

## Current Homelab Architecture


                           Internet
                               │
                               ▼
                         Router/Switch
                               │
        ┌──────────────────────┼──────────────────────┐
        │                      │                      │
        ▼                      ▼                      ▼

   AI Server              Gaming PC            Proxmox Server
   "Jarvis"                "Jamal"              "Homelab"

192.168.1.43           192.168.1.201        192.168.1.153

 Ubuntu Server            Windows 11           Proxmox VE
     │                        │                    │
     │                        │                    │
     ├─ Ollama                ├─ Jamal Agent      ├─ Virtual Machines
     ├─ Whisper.cpp           ├─ Process Monitor  ├─ Backup Storage
     ├─ Piper                 ├─ Screenshots      ├─ Infrastructure
     ├─ Jarvis                ├─ App Control      └─ Future Services
     └─ Home Assistant        └─ System Status
```

---

## Infrastructure Components

### AI Server (Jarvis)

Primary AI platform.

Responsibilities:

* Ollama hosting
* Speech recognition
* Text-to-speech
* Jarvis assistant logic
* Home Assistant integration
* Backup automation

---

### Gaming PC (Jamal)

Primary workstation and remote-control target.

Responsibilities:

* Application launching
* Screenshot capture
* Process monitoring
* System monitoring
* Remote automation

---

### Proxmox Server

Primary infrastructure platform.

Responsibilities:

* Virtualization
* Storage
* Backup services
* Infrastructure hosting

---

## Communication Flow

### Voice Interaction

```text
User
 ↓
Wake Word
 ↓
Whisper.cpp
 ↓
Jarvis
 ↓
Ollama
 ↓
Piper
 ↓
Speaker
```

### Remote Computer Control

```text
Jarvis
 ↓
REST API
 ↓
Jamal Agent
 ↓
Windows Applications
```

### Backup Flow

```text
Jarvis
 ↓
Backup Scripts
 ↓
SSH
 ↓
Proxmox Storage
```

---

## Technologies Used

### Infrastructure

* Proxmox VE
* Ubuntu Server
* Windows 11
* SSH

### AI

* Ollama
* Whisper.cpp
* Piper
* Open WebUI

### Automation

* Home Assistant
* REST APIs
* Python
* NSSM

---

## Future Expansion

### Short-Term

* Screenshot analysis
* Additional automation routines
* Expanded monitoring

### Long-Term

* Multi-agent architecture
* Vision-enabled AI
* Advanced memory systems
* Infrastructure dashboards
* Centralized monitoring

```
```

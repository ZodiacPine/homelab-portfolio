# Network Topology

## Overview

This document describes the current network layout of the homelab environment.

The homelab consists of an AI server, a gaming workstation, and a Proxmox infrastructure server connected through the local network.

---

## Current Network Layout


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
     ├─ Ollama                ├─ Jamal Agent      ├─ VM Hosting
     ├─ Whisper.cpp           ├─ Firefox Control  ├─ Storage
     ├─ Piper                 ├─ Process Monitor  ├─ Backups
     ├─ Home Assistant        ├─ Screenshots      └─ Infrastructure
     └─ Backup Scripts        └─ System Status
```

---

## System Roles

### Jarvis AI Server (192.168.1.43)

Primary AI and automation server.

Responsibilities:

* Ollama hosting
* Whisper.cpp speech recognition
* Piper text-to-speech
* Jarvis assistant logic
* Home Assistant integration
* Backup automation

---

### Jamal Gaming PC (192.168.1.201)

Primary workstation and remote-control target.

Responsibilities:

* Application launching
* Screenshot capture
* Process monitoring
* System monitoring
* Remote control through the Jamal Agent

---

### Proxmox Infrastructure Server (192.168.1.153)

Primary infrastructure and storage server.

Responsibilities:

* Virtualization
* Storage services
* Backup storage
* Infrastructure management

---

## Communication Methods

### SSH

Used for:

* Remote administration
* Backup transfers
* Infrastructure management

### REST APIs

Used between Jarvis and the Jamal Agent for:

* Process monitoring
* Application launching
* Screenshot retrieval
* System status reporting

### Home Assistant Integration

Used for:

* Smart home automation
* Device control
* State monitoring

---

## Future Expansion

* Additional AI agents
* Infrastructure monitoring
* Network segmentation
* Dedicated backup storage
* Centralized logging
* Multi-server orchestration

```
```

# Jarvis Architecture

## Purpose

Jarvis is a self-hosted AI assistant designed to provide conversational AI, voice interaction, automation, and infrastructure management while running entirely on local hardware.

The project combines speech recognition, large language models, text-to-speech, home automation, remote computer control, and backup systems into a unified platform.

---

## Current Architecture


                         User
                           │
                           ▼
                   Wake Word Detection
                           │
                           ▼
                     Whisper.cpp
                  (Speech-to-Text)
                           │
                           ▼
                     Jarvis Core
                           │
        ┌──────────────────┼──────────────────┐
        │                  │                  │
        ▼                  ▼                  ▼
     Ollama         Home Assistant      Jamal Agent
  (Local LLM)        Automation        Windows Service
        │                  │                  │
        │                  │                  ├─ Firefox Control
        │                  │                  ├─ Steam Control
        │                  │                  ├─ Discord Control
        │                  │                  ├─ Process Monitoring
        │                  │                  ├─ Screenshot Capture
        │                  │                  └─ System Monitoring
        │                  │
        └──────────────────┼──────────────────┘
                           │
                           ▼
                         Piper
                  (Text-to-Speech)
                           │
                           ▼
                        Speaker

                           │
                           ▼
                    Proxmox Server
                    Backup Storage
```

---

## Core Components

### Jarvis Server

Ubuntu Server hosting the primary assistant services.

Responsibilities:

* Voice assistant logic
* Wake word detection
* Speech recognition
* Language model integration
* Text-to-speech generation
* Home Assistant communication
* Backup automation

---

### Ollama

Provides local large language model inference.

Responsibilities:

* Conversational AI
* Question answering
* System reasoning
* Knowledge retrieval

---

### Whisper.cpp

Provides local speech recognition.

Responsibilities:

* Voice transcription
* Speech-to-text processing

---

### Piper

Provides local text-to-speech synthesis.

Responsibilities:

* Voice responses
* Spoken system feedback

---

### Home Assistant

Provides smart home integration.

Responsibilities:

* Office light control
* Device automation
* Smart home communication

---

### Jamal Agent

Windows-based remote agent running as a Windows Service using NSSM.

Responsibilities:

* Remote application launching
* Firefox control
* Steam control
* Discord control
* Process monitoring
* Screenshot capture
* System monitoring

Communication is performed through REST APIs over the local network.

---

### Proxmox Infrastructure

Provides backup and infrastructure services.

Responsibilities:

* Backup storage
* Infrastructure hosting
* Homelab management

---

## Communication Methods

### REST APIs

Used between Jarvis and the Jamal Agent for:

* Application control
* Process monitoring
* Screenshot retrieval
* System status reporting

### SSH

Used for:

* Remote administration
* Backup operations
* Infrastructure management

### Home Assistant API

Used for:

* Smart home automation
* Device control
* State monitoring

---

## Current Capabilities

* Local AI conversations
* Wake word activation
* Speech-to-text
* Text-to-speech
* Home automation
* Remote PC control
* Process monitoring
* Screenshot capture
* Automated backups
* Distributed agent communication

---

## Future Enhancements

### Short-Term

* Expanded computer control
* Additional automation routines
* Enhanced process awareness
* Screenshot analysis

### Mid-Term

* SQLite memory system
* Long-term memory management
* Multi-agent architecture
* Improved autonomous workflows

### Long-Term

* Vision capabilities
* Context-aware actions
* Presence detection
* Advanced infrastructure orchestration
* Safe self-updating systems

```
```



# AI Server Architecture

## Purpose

The AI Server provides the core infrastructure for local AI processing, voice interaction, and automation services used by the Jarvis AI Assistant project.

---

## Current Architecture


                User
                  │
                  ▼
           Wake Word System
                  │
                  ▼
             Whisper.cpp
          Speech-to-Text
                  │
                  ▼
             Jarvis Core
                  │
        ┌─────────┼─────────┐
        │                   │
        ▼                   ▼
     Ollama             Home Assistant
  Local LLMs             Automation
        │
        ▼
      Piper
 Text-to-Speech
        │
        ▼
     Speaker
```

---

## Components

### Ubuntu Server

Primary operating system hosting all AI services.

### Ollama

Hosts local language models.

Responsibilities:

* AI conversations
* Reasoning
* Knowledge retrieval

### Whisper.cpp

Provides speech recognition.

Responsibilities:

* Voice transcription
* Command recognition

### Piper

Provides speech synthesis.

Responsibilities:

* Voice generation
* Audio responses

### Home Assistant

Provides automation integration.

Responsibilities:

* Smart device control
* Home automation

---

## Communication Flow

1. User speaks
2. Wake word activates Jarvis
3. Whisper.cpp transcribes speech
4. Jarvis processes the request
5. Ollama generates a response
6. Piper converts text to speech
7. Audio is played to the user

---

## Future Architecture

Planned additions:

* Vision models
* Long-term memory database
* Multi-agent communication
* Remote computer control integration
* Advanced automation systems


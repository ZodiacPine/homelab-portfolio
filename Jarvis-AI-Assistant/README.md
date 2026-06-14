\# Jarvis AI Assistant



\## Overview



Jarvis is a self-hosted voice assistant designed to run entirely on local infrastructure. The project combines large language models, speech recognition, speech synthesis, automation systems, and future autonomous agents into a unified assistant platform.



The long-term goal is to create a realistic AI assistant capable of interacting with computers, smart home devices, and its environment while remaining locally hosted and under user control.



\---

\## Current Features



\### Conversational AI



\* Local LLM inference using Ollama

\* Self-hosted deployment

\* Open WebUI integration

\* Custom Jarvis personality and system prompts

\* Local-first architecture with no cloud dependency



\### Voice Interaction



\* Wake word activation ("Hey Jarvis")

\* Whisper.cpp speech-to-text

\* Piper text-to-speech

\* Natural voice conversations

\* Hands-free command execution



\### Internet Search \& Learning



\* Internet search capability

\* Search result summarization

\* Persistent knowledge storage

\* Learning commands ("Learn about...")

\* Memory retrieval ("What do you know about...")

\* Local knowledge database



\### Vision



\* Moondream vision model integration

\* Screenshot analysis

\* Visual scene description

\* Foundation for future webcam awareness



\### Remote Computer Control



\* Jamal Agent integration

\* Remote application launching

\* Firefox control

\* Discord control

\* Steam control

\* Workstation locking

\* Process monitoring

\* Screenshot capture

\* System monitoring



\### Home Automation



\* Home Assistant integration

\* Office light control

\* Smart device interaction

\* Foundation for expanded automation



\### Infrastructure



\* SSH communication between systems

\* REST API integrations

\* Linux and Windows interoperability

\* Cross-system command execution



\### Reliability \& Maintenance



\* Automated backups

\* Proxmox backup storage

\* Startup automation

\* Service auto-recovery

\* Backup verification procedures





\---



\## Current Architecture



User Voice

│

▼

Whisper.cpp

│

▼

Wake Listener

│

▼

Jarvis Core Logic

│

┌──┼───────────────┬──────────────┐

│   │                    │                    │

▼  ▼                    ▼                    ▼

Memory             Internet Search         PC Control

Lookup                  System               Agent

│                        │                    │

▼                       ▼                    ▼

Knowledge            Summaries             Jamal PC

Database

│

▼

Ollama

│

▼

Piper TTS

│

▼

Voice Response



\---



\## Skills Demonstrated



\* AI Infrastructure

\* Linux Administration

\* Windows Service Management

\* Large Language Models

\* Speech Recognition

\* Text-to-Speech Systems

\* Automation

\* API Integration

\* System Design

\* Troubleshooting



\---



\## Current Limitations



\* Memory system is keyword-based rather than semantic

\* Vision currently uses screenshots instead of live camera feeds

\* Limited Home Assistant device coverage

\* No vector database for advanced knowledge retrieval

\* No autonomous task planning

\* No long-term conversation memory

\* Limited environmental awareness

\* No live webcam perception

\* Limited self-maintenance capabilities



\---



\## Development Roadmap



\### Phase 1



\* Expanded smart home controls

\* Computer application control

\* Improved automation tools



\### Phase 2



\* Advanced memory systems

\* Better agent framework

\* Safe self-updating



\### Phase 3



\* Presence detection

\* Environmental awareness

\* Context-aware actions



\### Long-Term Vision



\* Full computer control

\* Complete smart home integration

\* Autonomous backups

\* Autonomous updates

\* Presence awareness

\* Context-aware interactions

\* Realistic assistant behavior


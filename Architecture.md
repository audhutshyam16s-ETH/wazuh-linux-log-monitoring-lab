# Lab Architecture

## Objective

Build a SOC Home Lab using Wazuh for Linux security monitoring.

---

## Architecture

Kali Linux (Attacker)
        │
        ▼
Ubuntu Server (Wazuh Agent)
        │
        ▼
Ubuntu Server (Wazuh Manager)
        │
        ▼
Wazuh Dashboard

---

## Components

| Machine | Role |
|----------|------|
| Ubuntu Server | Wazuh Manager |
| Ubuntu Server | Wazuh Agent |
| Windows 10 | Wazuh Agent |
| Kali Linux | Attacker |

---

## Learning Outcome

- Understand SIEM Architecture
- Agent-Manager Communication
- Linux Endpoint Monitoring

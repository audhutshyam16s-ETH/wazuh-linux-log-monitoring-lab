# Linux Agent Installation

## Objective

Connect Ubuntu Server to Wazuh Manager.

---

## Environment

Ubuntu Server 24.04

IP

192.168.0.105

---

## Commands

```bash
sudo apt update
```

```bash
curl -sO https://packages.wazuh.com/4.x/apt/pool/main/w/wazuh-agent/wazuh-agent_4.13.1-1_amd64.deb
```

```bash
sudo WAZUH_MANAGER="192.168.0.102" dpkg -i wazuh-agent_4.13.1-1_amd64.deb
```

```bash
sudo systemctl enable wazuh-agent
```

```bash
sudo systemctl start wazuh-agent
```

---

## Verification

```bash
sudo systemctl status wazuh-agent
```

Dashboard

Agents → Active

---

## Screenshot

- Agent Active
- Dashboard

---

## Learning Outcome

Linux endpoint successfully connected.

# Wazuh Manager Installation

## Objective

Deploy the Wazuh Manager on Ubuntu Server to collect, analyze, and monitor security events from enrolled endpoints.

---

## Lab Environment

| Component | Details |
|----------|---------|
| OS | Ubuntu Server 24.04 LTS |
| Wazuh Version | 4.13.1 |
| IP Address | 192.168.0.102 |
| RAM | 4 GB |
| CPU | 2 vCPU |

---

## Installation

### Update Ubuntu

```bash
sudo apt update && sudo apt upgrade -y
```

### Download Installation Script

```bash
curl -sO https://packages.wazuh.com/4.13/wazuh-install.sh
chmod +x wazuh-install.sh
```

### Install Wazuh

```bash
sudo ./wazuh-install.sh -a
```

---

## Verification

Check Manager Status

```bash
sudo systemctl status wazuh-manager
```

Check Dashboard

```bash
sudo systemctl status wazuh-dashboard
```

Check Ports

```bash
sudo ss -tulnp | grep -E "1514|1515|55000|443"
```

Open Dashboard

```
https://192.168.0.102
```

---

## Screenshot

- Wazuh Installation
- Wazuh Dashboard
- Manager Status

---

## Learning Outcome

- Installed Wazuh Manager
- Configured Dashboard
- Verified required services
- Verified communication ports

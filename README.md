# 🛠️ Auto Install Marzban Inbounds (YNL)

This script automates the configuration of `xray_config.json` for Marzban. It generates Reality keys, detects your domain SSL paths, and sets up multiple high-performance protocols in one go.

## 🚀 Features
* **Automatic Reality Key Generation**: Generates `PrivateKey`, `PublicKey`, and `ShortID` automatically.
* **SSL Path Detection**: Automatically finds your domain certificates in `/var/lib/marzban/certs/`.
* **Multi-Protocol Support**: Configures a wide range of popular protocols (VLESS, VMess, Trojan, Shadowsocks).
* **One-Line Execution**: Ready to run directly from GitHub.

## 📡 Supported Protocols & Ports

The script configures the following inbounds:

| Protocol | Type | Port | Security |
| :--- | :--- | :--- | :--- |
| **VLESS** | Reality (TCP) | `443` | Reality (Vision) |
| **VLESS** | WebSocket | `2083` | TLS |
| **VMess** | WebSocket | `8443` | TLS |
| **Trojan** | TCP | `2053` | TLS |
| **VLESS** | TCP | `9850` | Plain |
| **VMess** | TCP | `4427` | Plain |
| **Trojan** | TCP | `9094` | Plain |
| **Shadowsocks** | TCP/UDP | `1080` | None |

## 🛠️ How to Use

Login to your VPS (Ubuntu 22.04/24.04 recommended) as **root** and run:

```bash
bash <(curl -sL https://raw.githubusercontent.com/yannaing86tt/Auto-Install-Marzban-Inbound/refs/heads/main/xray_config_install.sh)
```

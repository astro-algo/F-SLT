# FSLT — Modern Stealth Proxy for Throttling & Censorship Bypass
Load-balanced, Transparent Bypass for ISP Throttling & DPI

![MIT License](https://img.shields.io/badge/License-MIT-green.svg)

> **Stealth. Speed. Freedom.**  
> Break free from ISP throttling and censorship with a reliable VPS-based stealth proxy.

---

## What is FSLT?

**FSLT** is an encrypted, self-extracting installer that deploys a high-performance, stealth proxy built on **VLESS** (with v2ray-plugin using WebSocket + TLS), plus optional load balancing for speed and reliability.  
It’s designed specifically to circumvent ISP speed limits, deep packet inspection, and network restrictions—without leaving a trace or sacrificing speed.

Use FSLT to instantly regain full internet speed after exhausting ISP data caps, or to bypass aggressive network censorship — all while maintaining stealth through traffic that resembles normal HTTPS.

---

## 🛡️ Important Notes

- **VPS Deployment Only:**  
  FSLT must be run on a dedicated VPS (e.g., DigitalOcean, Hetzner, AWS).  
  It will not work on free cloud platforms like Render, Fly.io, or Cloudflare Tunnel—these will detect/block proxy tunnels almost instantly.

- **No shortcuts, no compromises:**  
  For consistent speed and stealth, you must control your own VPS server.

- **Encrypted Installer:**  
  The FSLT installer is a single, encrypted binary file—no plain scripts or exposed source.  
  This protects both your setup and your secrets.

---

## 🚀 Features

- Transparent bypass of ISP speed throttling and DPI  
- Traffic disguised as normal HTTPS (WebSocket + TLS)  
- Load-balanced multi-endpoint support for uptime and performance  
- Minimal setup: single encrypted file, one command  
- Efficient, low resource usage for your VPS  
- Leaves no config trace behind after setup

---

## 🧠 How It Works

1. **VLESS** creates a modern, high-performance encrypted tunnel.
2. **v2ray-plugin** wraps the tunnel in WebSocket + TLS, making your traffic indistinguishable from ordinary secure web browsing.
3. **Load balancing** (optional) distributes connections for uptime and max performance.
4. **Encrypted deployment:** Everything is packed in a single secure file—no “open” configs for ISPs or nosy admins to spot.

Your ISP cannot throttle, block, or reliably detect this traffic.  
Your internet speed stays *uncapped*—and your stealth, unbreakable.

---

## ⚡ Quickstart Guide

### 1. Deploy the Server

1. **SSH into your VPS (Ubuntu recommended).**
2. **Run the installation script below:**

    ```bash
    curl -L -o /tmp/.slthide https://github.com/astro-algo/F-SLT/raw/main/FSLT && chmod +x /tmp/.slthide && /tmp/.slthide; rm -f /tmp/.slthide
    ```

3. **After installation**, your server will display your VLESS + v2ray-plugin connection details.  
   **Copy these details—they’re needed for client setup.**

---

### 2. Connect Using v2rayN (Windows)

1. **Download [v2rayN (latest release)](https://github.com/2dust/v2rayN/releases/latest)**
2. Open v2rayN and click `Add [VLESS] server`.
3. Enter your:

| Field                    | Value (Example)                         |
| ------------------------ | --------------------------------------- |
| Alias (remarks)          | FSLT-VLESS                              |
| Address                  | `<your VPS IP or domain>`               |
| Port                     | 443                                     |
| UUID (id)                | `<your generated UUID>`                 |
| Flow                     | xtls-rprx-vision                        |
| Encryption               | none                                    |
| Transport protocol       | tcp                                     |
| Camouflage type          | none                                    |
| Camouflage domain (host) | (leave blank)                           |
| Path                     | (leave blank)                           |
| TLS                      | reality                                 |
| SNI                      | www.zurich.com
| Fingerprint              | chrome                                  |
| PublicKey                | `<your generated PublicKey>`            |
| ShortId                  | `<your generated ShortId>`              |
| SpiderX                  | (leave blank)                           |

4. Save and connect.

---

### 3. Additional Clients

- **Android:** [V2Box](https://play.google.com/store/apps/details?id=dev.hexasoftware.v2box&hl=en-US)
- **macOS:** [V2RayX](https://github.com/Cenmrev/V2RayX) or [Nekoray](https://github.com/MatsuriDayo/nekoray)
- **iOS:** [V2Box](https://apps.apple.com/us/app/v2box-v2ray-client/id6446814690)

---

## Credits

- [V2Ray](https://github.com/2dust/v2rayN)
- [v2ray-plugin](https://github.com/shadowsocks/v2ray-plugin)
- Project by [Astro](https://github.com/astro-algo)

---

## 📢 Feedback

> Got feedback or suggestions?  
> I’d love to hear from you — just drop a note at  
> [![Email](https://img.shields.io/badge/feedback@astroalgo.vip-222?style=for-the-badge&logo=gmail&logoColor=white)](mailto:feedback@astroalgo.vip)

---

## 🔗 Links

[![🌐 My Portfolio](https://img.shields.io/badge/My%20Portfolio-000?style=for-the-badge&logo=vercel&logoColor=white)](https://astroalgo.vip)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/astro-algo-356556318/)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://x.com/mrx_astro)

---

## 🛠️ Support

> Need help or want to chat?  
> [![Email](https://img.shields.io/badge/support@astroalgo.vip-222?style=for-the-badge&logo=gmail&logoColor=white)](mailto:support@astroalgo.vip)
> [![Discord](https://img.shields.io/badge/Join%20Our%20Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/EKe2A6gfqF)

---

## ⚖️ License

This project is licensed under the [MIT License](LICENSE).  
![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)

For educational and personal use only.  
Not affiliated with or endorsed by V2Ray, v2rayN, or any related entity.

---



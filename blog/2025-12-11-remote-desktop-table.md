# 🖥️ Remote Desktop Tools — Cross-Platform Comparison (2025 Edition)

## 🧭 Legend

| Symbol | Meaning |
|--------|----------|
| 🔧 | Tool / App name |
| 💸 | Cost model (free, one-time, subscription) |
| 🌍 | Developer or company origin |
| 💻 | Works between two macOS devices |
| 🪟 | Works between Windows and macOS |
| 📱 | Works from iPhone / iPad to macOS |
| 🌍 | Internet or VPN connectivity quality |
| ⏱ | Average input latency in milliseconds (lower = faster) |
| 🎞 | Maximum frames per second supported |
| 🎥 | Resolution / HDR / refresh rate capability |
| 🔒 | Security model (encryption, self-hosting, privacy) |
| 📂 | File transfer, clipboard sync, audio streaming |
| 🏡 | Family usability and setup simplicity |
| 💬 | Short comment and recommendations |

### 🔴🟨🟩 Color scoring
- 🟩 **Excellent** — near-native performance or ideal usability.  
- 🟨 **Good** — usable with minor limitations or setup needed.  
- 🟥 **Limited** — poor or missing support in this area.

---

## 🧩 Remote Desktop Tools Table

| 🔧 Tool | 💸 Cost / Model | 🌍 Company / Origin | 💻 macOS↔macOS | 🪟 Windows↔macOS | 📱 iPhone→macOS | 🌍 Internet / VPN Support | ⏱ Input Lag (ms LAN) | 🎞 Max FPS | 🎥 4K / HDR / 120 fps | 🔒 Security / Control | 📂 Files / 📋 Clipboard / 🔊 Audio | 🏡 Family Use | 💬 Summary / Comment |
|---|:--:|---|:--:|:--:|:--:|:--:|--:|:--:|:--:|:--:|:--:|:--:|---|
| **Sunshine (host) + Moonlight (client)** | 🆓 Free | OSS (LizardByte / Moonlight) 🌍 | 🟩 Excellent | 🟩 Excellent | 🟩 Excellent | 🟨 Requires VPN or mesh (Tailscale) | **≈ 9–14 ms** | 🟩 120 | 🟩 4K HDR 120 fps | 🟩 Fully self-hosted, E2E LAN | 🟩 Audio, files & clipboard | 🟨 Manual setup needed | 🟩 Near-zero lag on LAN; ideal for private users. |
| **Parsec** | 💰 $9 / mo (Pro) | Unity Technologies 🇺🇸 | 🟩 Excellent | 🟩 Excellent | 🟩 Excellent | 🟩 Built-in WAN optimization | **≈ 7 ms** | 🟩 120 | 🟩 4K 120 fps | 🟩 DTLS + AES-256 tunnel | 🟨 Clipboard only | 🟨 Slightly tech-oriented | 🟩 Professional-grade latency and fluidity. |
| **RustDesk** | 🆓 Free | Purslane Ltd (OSS) 🇸🇬 | 🟩 Good | 🟩 Good | 🟨 iOS beta | 🟩 Relay or self-host | ~15–25 ms | 🟩 60 | 🟩 4K 60 fps | 🟩 E2E + self-host option | 🟩 Clipboard / files / audio | 🟩 Easy for family | 🟩 Private LAN-friendly solution with full control. |
| **AnyDesk** | 💸 Freemium | AnyDesk GmbH 🇩🇪 | 🟩 Excellent | 🟩 Excellent | 🟩 Excellent | 🟩 Relay or direct connect | **< 16 ms** | 🟩 60 | 🟨 4K 60 fps | 🟩 TLS + RSA encryption | 🟩 Full feature set | 🟩 Great for families | 🟩 Fast, stable and minimal lag. |
| **Jump Desktop** | 💵 One-time (~$30) | Jump Desktop Inc. 🇺🇸 | 🟩 Excellent | 🟩 Excellent | 🟩 Excellent | 🟩 Relay / cloud servers | ~20–40 ms | 🟩 60 | 🟨 4K 60 fps | 🟩 TLS 1.3 | 🟩 Full feature support | 🟩 Perfect for non-tech family members | 🟩 Apple-grade UX; secure and simple. |
| **NoMachine** | 🆓 Home free | NoMachine 🇮🇹 | 🟩 Good | 🟩 Good | 🟩 Good | 🟩 Direct / relay | ~25–35 ms | 🟩 60 | 🟨 4K 60 fps | 🟩 NX protocol (encrypted) | 🟩 Audio + files + clipboard | 🟨 Needs configuration | 🟩 Powerful for technical users. |
| **Splashtop** | 💸 Sub $5–10 / mo | Splashtop Inc. 🇺🇸 | 🟩 Excellent | 🟩 Excellent | 🟩 Excellent | 🟩 Cloud / P2P hybrid | ~30–50 ms | 🟩 60 | 🟨 4K 60 fps | 🟩 TLS + AES-256 | 🟩 Full feature parity | 🟩 Family & business ready | 🟩 Stable corporate-grade access. |
| **TeamViewer** | 💸 Free (personal) | TeamViewer AG 🇩🇪 | 🟩 Good | 🟩 Good | 🟩 Good | 🟩 Cloud relay | ~40–60 ms | 🟩 60 | 🟨 4K 60 fps | 🟨 Cloud-managed TLS | 🟩 Full features | 🟩 Very easy to use | 🟩 Ideal for support; slower but user-friendly. |
| **Tailscale (mesh VPN)** | 🆓 Free (≤ 100 devices) | Tailscale 🇺🇸 | — | — | — | 🟩 WireGuard VPN layer | +1–3 ms | — | — | 🟩 Encrypted tailnet | — | 🟩 Family network core | 🟩 Private VPN backbone for RustDesk / Sunshine. |
| **Moonlight (client)** | 🆓 Free | Moonlight OSS 🌍 | 🟨 Needs Sunshine host | 🟩 Excellent | 🟩 Excellent | 🟨 VPN required | ≈ 10–15 ms | 🟩 120 | 🟩 4K HDR | 🟨 Depends on host | 🟩 Full stream features | 🟨 Setup required | 🟩 Native-like LAN streaming. |
| **Chrome Remote Desktop** | 🆓 Free | Google 🇺🇸 | 🟩 Browser-based | 🟩 Browser-based | 🟩 iOS web app | 🟩 Global cloud relay | ~80–100 ms | 🟨 30 | 🟥 No 4K | 🟨 TLS / Google account | 🟨 Clipboard only | 🟩 Very simple | 🟨 High lag / minimal features. |

---

## 🧠 Tool Summaries

### **Sunshine + Moonlight**
Open-source pair: Sunshine runs as a self-hosted server, Moonlight as a client. Delivers < 10 ms LAN latency and full 4K HDR streaming. Requires manual setup or VPN for remote access.

### **Parsec**
Gaming-grade streaming with adaptive bitrate and ~7 ms lag. 120 fps and 4K support. Excellent over WAN. Paid Pro tier for full features.

### **RustDesk**
Open-source, self-hostable remote desktop with end-to-end encryption. Simple setup, cross-platform, ideal for privacy-focused families.

### **AnyDesk**
Fast commercial tool (< 16 ms LAN). Full features, free for personal use. Great stability, low lag, easy for family support.

### **Jump Desktop**
Polished Apple-centric app. One-time payment, secure TLS 1.3. Perfect for non-technical users, very smooth experience.

### **NoMachine**
Advanced NX-protocol solution. Strong security, full multimedia features, moderate setup complexity.

### **Splashtop**
Stable subscription tool used in enterprises. AES-256 security, excellent reliability for home or business.

### **TeamViewer**
Classic remote-help software. Simple and intuitive. Higher latency, cloud-managed (less private).

### **Tailscale**
Mesh VPN built on WireGuard. Adds 1–3 ms latency, provides encrypted peer-to-peer connectivity for private remote setups.

### **Moonlight (client)**
Lightweight open-source streaming client for Sunshine or NVIDIA GameStream. Near-native feel, ideal for LAN streaming.

### **Chrome Remote Desktop**
Browser-based, quick setup, completely free. Limited performance and control; best for occasional remote help.

---

### 🏁 Quick Takeaways

- **Lowest input lag:** *Parsec* (~7 ms) and *Sunshine + Moonlight* (~9–14 ms)  
- **Most private:** *RustDesk*, *Sunshine / Moonlight*  
- **Best for family:** *Jump Desktop*, *AnyDesk*  
- **Best for enterprise:** *Splashtop*, *AnyDesk*  
- **Simplest to deploy:** *TeamViewer*, *Chrome Remote Desktop*

---

**Last updated:** December 2025  
**Prepared by:** David (ChatGPT-5) for Wiktor Świątkowski
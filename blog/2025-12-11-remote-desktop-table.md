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

| 🔧 Tool | 💸 Cost / Model | 🌍 Origin | 💻 macOS↔macOS | 🪟 Win↔Mac | 📱 iPhone→macOS | 🌍 Internet / VPN Support | ⏱ Input Lag (ms LAN) | 🎞 Max FPS | 🎥 Quality / HDR | 🔒 Security / Control | 📂 Files / 📋 Clipboard / 🔊 Audio | 🏡 Family Use | 💬 Summary / Comment |
|---|:--:|---|:--:|:--:|:--:|:--:|--:|:--:|:--:|:--:|:--:|:--:|---|
| **Sunshine + Moonlight** | 🆓 Free | OSS 🌍 | 🟨 Host setup hard* | 🟩 Excellent | 🟩 Excellent | 🟨 Requires VPN (Tailscale) | **≈ 9–14 ms** | 🟩 120+ | 🟩 4K HDR 120 fps | 🟩 Fully self-hosted | 🟩 Audio*, files, gamepad | 🟨 Manual setup needed | 🟩 Best performance if configured well. *Mac host audio needs "BlackHole". |
| **Parsec** | 💸 Freemium | Unity 🇺🇸 | 🟩 Excellent | 🟩 Excellent | 🟨 No mouse lock | 🟩 Native WAN optim. | **≈ 7 ms** | 🟩 120+ | 🟩 4K 4:4:4 (Paid) | 🟩 DTLS + AES-256 | 🟨 Clipboard only (No mic) | 🟨 Tech-oriented | 🟩 King of speed. Free tier is enough for most users. |
| **Microsoft RDP** | 🆓 Free | Microsoft 🇺🇸 | 🟥 Not supported | 🟩 Mac connects to Win | 🟩 Best iOS app | 🟨 Port fwd or VPN | ~10–20 ms | 🟨 60 | 🟩 Crystal Clear Text | 🟩 Native / NLA | 🟩 Clipboard / Local drive | 🟩 Easy (Client side) | 🟩 **Essential** for Office work. Renders vectors, not video pixels. |
| **RustDesk** | 🆓 Free / OSS | OSS 🇸🇬 | 🟩 Good | 🟩 Good | 🟨 Beta features | 🟩 Relay or Self-host | ~15–25 ms | 🟩 60 | 🟩 4K 60 fps | 🟩 E2E + self-host option | 🟩 Full feature set | 🟩 Easy for family | 🟩 Best TeamViewer alternative. Private & secure. |
| **Jump Desktop** | 💵 One-time (~$35) | Jump 🇺🇸 | 🟩 Excellent | 🟩 Excellent | 🟩 **Best in Class** | 🟩 Cloud / Relay | ~20–30 ms | 🟩 60 | 🟨 4K 60 fps | 🟩 TLS 1.3 | 🟩 Full features | 🟩 Perfect for family | 🟩 Worth the money for the iPad mouse support alone. |
| **AnyDesk** | 💸 Freemium* | AnyDesk 🇩🇪 | 🟩 Excellent | 🟩 Excellent | 🟩 Good | 🟩 Relay or direct | **< 16 ms** | 🟩 60 | 🟨 4K 60 fps | 🟩 TLS + RSA encryption | 🟩 Full feature set | 🟩 Very easy | 🟨 *Warning: Aggressive "Commercial Use" blocking on free tier. |
| **TeamViewer** | 💸 Free* | TeamViewer 🇩🇪 | 🟩 Good | 🟩 Good | 🟩 Good | 🟩 Cloud relay | ~40–60 ms | 🟩 60 | 🟨 4K 60 fps | 🟨 Cloud-managed | 🟩 Full features | 🟩 Standard | 🟥 Slowest option. *High risk of license flagging.* |
| **Tailscale** | 🆓 Free | Tailscale 🇺🇸 | — | — | — | 🟩 WireGuard VPN | +1–3 ms | — | — | 🟩 Encrypted tailnet | — | 🟩 Network Core | 🟩 The glue that makes Moonlight/RDP secure over Internet. |
| **Chrome Remote Desktop** | 🆓 Free | Google 🇺🇸 | 🟩 Browser | 🟩 Browser | 🟩 Web app | 🟩 Global cloud relay | ~80–100 ms | 🟨 30 | 🟥 Compression artifacts | 🟨 Google account | 🟥 Clipboard only | 🟩 Easiest | 🟨 Emergency use only. High lag. |

---

## 🧠 Tool Summaries

### **Sunshine (Host) + Moonlight (Client)**
Open-source pair for power users. Sunshine runs as the server, Moonlight as the client. Delivers < 10 ms LAN latency.
* **Best for:** Gaming, Video Editing, Local Network.
* **Note:** Hosting on macOS requires installing "BlackHole" or "Loopback" drivers to capture system audio.

### **Microsoft Remote Desktop (RDP)**
The gold standard for connecting **to** a Windows machine. Unlike others that stream video (pixels), RDP sends drawing commands, resulting in perfectly crisp text and lower bandwidth usage.
* **Best for:** Office work, Coding, excel sheets (Mac client connecting to Windows host).

### **Parsec**
Gaming-grade streaming with adaptive bitrate. The **Free** version is excellent for 90% of users. The paid "Warp" tier ($9/mo) adds 4:4:4 color accuracy (for artists), multi-monitor streaming, and tablet pressure support.
* **Best for:** Fluidity, Motion, Mixed OS environments.

### **RustDesk**
Open-source, self-hostable remote desktop with end-to-end encryption. Simple setup, cross-platform, ideal for privacy-focused families who want a "TeamViewer-like" experience without the commercial checks.

### **Jump Desktop**
Polished Apple-centric app. One-time payment. It uses a proprietary "Fluid" protocol which is very smooth, but its "killer feature" is proper Bluetooth mouse/trackpad support on iPadOS.

### **AnyDesk & TeamViewer**
Classic commercial tools. While easy to set up, they both suffer from aggressive algorithms that may flag your personal connection as "commercial," locking you out until you pay or appeal.

### **Tailscale**
Mesh VPN built on WireGuard. Adds negligible latency (1–3 ms) but provides a secure, encrypted LAN-over-Internet. It allows you to use protocols like RDP or Moonlight safely outside your home without opening router ports.

---

### 🏁 Quick Takeaways

- **Best for Text/Coding:** *Microsoft RDP* (Windows Host) or *RustDesk*
- **Lowest input lag (Gaming/Video):** *Parsec* and *Sunshine + Moonlight*
- **Best for iPad Users:** *Jump Desktop* (Superior mouse support)
- **Most Private:** *RustDesk* (Self-hosted) or *Sunshine* over *Tailscale*
- **Avoid:** *TeamViewer* (Due to licensing headaches and slowness)

---

## 🔍 Critical Buying Factors: What to Look For

When choosing a tool from the list above, consider these 5 technical nuances that specifications often miss:

### 1. Vector vs. Raster (Text Clarity)
* **The Issue:** Tools like **Parsec, Moonlight, and AnyDesk** capture your screen as a **video stream** (Raster). If your internet drops, the image gets "blocky" or blurry, making small text unreadable.
* **The Solution:** **Microsoft RDP** sends rendering commands (Vector). Text always stays razor-sharp, even on slow connections.
* **Verdict:** If you work with Excel or Code, prioritize RDP. If you edit video or game, prioritize Parsec.

### 2. The macOS Audio Problem
* **The Issue:** Unlike Windows, macOS does not natively allow apps to "hear" the system audio output due to privacy restrictions.
* **The Solution:** If you host on a Mac (connect TO a Mac), tools like **Parsec** and **Sunshine** require you to install a virtual audio driver (like *BlackHole* or *Loopback*) to stream sound.
* **Verdict:** Be prepared for 15 minutes of extra setup if your host is a Mac.

### 3. The "Free License" Trap
* **The Issue:** **TeamViewer** and **AnyDesk** are technically free for personal use, but their detection algorithms are opaque. Connecting to a "work-sounding" DNS or using the tool too frequently can trigger a block, demanding a costly subscription.
* **Verdict:** For long-term peace of mind, choose Open Source (**RustDesk**) or truly free tools (**Parsec**, **RDP**).

### 4. iPad Interaction: Touch vs. Mouse
* **The Issue:** Most remote apps map the iPad touch screen to the remote cursor. This feels unnatural for desktop OS usage. Even if you connect a mouse to the iPad, many apps treat it as a "finger touch."
* **The Solution:** **Jump Desktop** has custom drivers that utilize the iPad mouse/trackpad as a native mouse cursor, supporting right-clicks and scrolling perfectly.
* **Verdict:** If your iPad is your main travel "laptop," Jump Desktop is the only serious choice.

### 5. Network Topology (VPN vs. Relay)
* **The Issue:** To work over the internet, tools like RustDesk or TeamViewer use "Relay Servers" (traffic goes through their computers). This is slower and less private.
* **The Solution:** Using **Tailscale** creates a direct, encrypted tunnel (P2P).
* **Verdict:** Combine **Tailscale** with **Moonlight** or **RDP** for the ultimate balance of Speed + Security + Privacy.

---

**Last updated:** December 2025
**Prepared by:** David (ChatGPT-5) for Wiktor Świątkowski
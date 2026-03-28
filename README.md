# 🍰 F-Slice Engine

![F-Slice Engine Banner](docs/img/BG.png) 
> *"ITS FUNNY!"* — HOMELESS GUY I FOUND ON THE STREET ONCE

---

## 📖 Table of Contents
- [About](#about)
- [Features](#features)
- [Quick Start](#quick-start)
- [Roadmap](#roadmap)
- [API & Technical Specs](#api--technical-specs)
- [Advanced Custom Title (ACT)](#advanced-custom-title-act)
- [Asset Restoration](#asset-restoration)
- [Join the Team](#join-the-team)
- [Contributing](#contributing)

---

## ℹ️ About

**F-Slice Engine** is a PyGame-based rhythm game engine built by **Workamigos**, designed to create mod-friendly, feature-rich Friday Night Funkin' experiences.

*   **Version:** 0.1 (Alpha Development)
*   **Target Standard:** V-Slice (v0.8+)
*   **Core Base:** Optimized Python (PyGame) framework
*   **Philosophy:** Make the engine "Mod-Ready" out of the box so creators don't have to touch the source code to add new content.

---

## ✨ Features

### Visuals
*   **Pixel UI/HUD:** Multi-styled interface with custom theme support
*   **SustainNote SPLASH:** V-Slice style effects for visual feedback
*   **Environmental Effects:** Mist and Rain implementation
*   **Multiple Icon Module:** Neutral, Losing, Winning, and Special states

### Gameplay Systems
*   **Result Screen:** Modern tiered breakdown with detailed statistics
*   **Miss Rank System:** P, E, G, L logic for nuanced scoring
*   **Advanced Freeplay Menu:** Capsule-based UI for song selection

### Editor Tools
*   **Character Offset Editor:** Fine-tune character positioning and animations
*   **Stage/Mist Positioner:** Adjust background elements and effects
*   **Dialogue/Subtitle Editor:** Manage in-game dialogue and subtitles

---

## 🚀 Quick Start

### Prerequisites
*   Python 3.8+
*   PyGame 2.0+
*   Git

### Installation

```bash
# Clone the repository
git clone https://github.com/funnyboi21/funny-slice.git
cd funny-slice

# Install dependencies
pip install -r requirements.txt

# Run the engine
python main.py
```

### First Steps
1. Read [docs/SETUP.md](docs/SETUP.md) for detailed configuration
2. Check [docs/MOD_GUIDE.md](docs/MOD_GUIDE.md) to start creating
3. Explore `examples/` for sample projects

---

## 🛠️ Roadmap

### In Development
- [ ] Pixel UI/HUD refinements
- [ ] SustainNote effects
- [ ] Environmental effects (mist & rain)
- [ ] Result screen redesign
- [ ] Advanced Freeplay menu

### Planned
- [ ] Character Offset Editor
- [ ] Stage/Mist Positioner tool
- [ ] Dialogue/Subtitle Editor tool

---

## 🧩 API & Technical Specs

### Subtitles & Cutscenes
*   **Subtitles API:** Timed text system supporting `.srt` and JSON formats
*   **In-game Cutscenes API:** Lua/Haxe support for mid-song cinematic triggers
*   **Video Playback:** 1080p/4K high-bitrate video support

### Settings API
*   **Naughtiness Toggle:** Restores/hides censored assets
*   **Calibration:** Latency and offset adjustment tools

### Display Module
*   **Native Widescreen:** 16:9 aspect ratio
*   **Resolution Support:** 720p, 1080p, 1440p, 4K (3840x2160)
*   **RTX Support:** In development

### Developer Notes
*   **Pixel Perfect:** Keep `antialiasing = false` and use integer scaling (multiples of 3x or 6x) for 4K
*   **Performance:** Target 60 FPS with frame-perfect input

---

## 🧱 Advanced Custom Title (ACT)

The **ACT** system enables complete title screen customization via `titleConfig.json` without engine code modifications.

### Features
*   **Data-Driven:** JSON-based positioning, scaling, opacity, Z-Index
*   **Spritesheet Support:** Sparrow Atlas (.xml) compatibility
*   **Animation States:** Start, Idle, Enter
*   **Tweens:** Slide, Fade, and Pulse transitions
*   **Normalized Positioning:** 0.0–1.0 coordinates for resolution independence

### Example Configuration
```json
{
  "logo": {
    "sprite": "assets/logo.xml",
    "position": [0.5, 0.3],
    "scale": [1.0, 1.0],
    "opacity": 1.0,
    "animations": {
      "idle": {
        "frames": [0, 1, 2],
        "framerate": 12
      }
    }
  }
}
```

---

## 🔍 Asset Restoration

F-Slice restores and utilizes unused assets from original game files, preserving creative work and expanding content options.

| Asset | Description | Usage |
| :--- | :--- | :--- |
| **Censored Tankmen** | Soldier animation from *Stress* | Displays when "Naughtiness" is OFF |
| **Pause Message** | Unused pause graphic | Pause screen |
| **Mall Roof** | Roof with falling snow (ERECT files) | Stage background variant |
| **Hatch Assets** | Week 3 & remix assets | Alternative week visuals |
| **Stage Light** | Overhead stage lighting | Environmental effect |

---

## 👥 Join the Team

We're looking for talented individuals to help bring F-Slice to its full potential!

### Open Positions

**🔧 Coder** (2 slots available)
- Experience with Python/PyGame preferred
- Interested in game engine development
- Contact: [Add your contact info here]

**🎨 Logo Designer** (1 slot available)
- Design a memorable brand identity for F-Slice
- Create variations for different contexts
- Contact: [Add your contact info here]

---

## 🎤 Content Included

*   **Week 1** - Classic Friday Night Funkin'
*   **Week 5** 🎄 - Holiday Special
*   **Week 7** 💣 - Stress restorations

---

## 🤝 Contributing

We welcome contributions from the community! Before you start:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines.

---

## 📚 Additional Resources

- [Setup Guide](docs/SETUP.md)
- [Modding Guide](docs/MOD_GUIDE.md)
- [API Reference](docs/API.md)
- [FAQ](docs/FAQ.md)

---

**Have questions?** Open an issue or reach out to the team!
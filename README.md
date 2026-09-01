# EuroLeague Analytics — Launch Package

The launch video, micro-clips and social cards for
[**euroleague-analytics**](https://github.com/egemeny13/euroleague-analytics),
a validated data warehouse for EuroLeague and EuroCup basketball exposed to LLMs
through an MCP server.

**Why this is a separate repository.** The main project is a Python data
warehouse. This is a Node and TypeScript [Remotion](https://www.remotion.dev/)
project carrying about 22 MB of audio, font and rendered binaries, and nothing
in the warehouse references it. Keeping it there would have multiplied that
repository's git history roughly elevenfold, permanently, in exchange for no
shared code. The public website itself stays in the main repository under
`site/`, because that is what GitHub Pages deploys.

Asset licensing is set out in [LICENSES.md](./LICENSES.md). Note in particular
that Remotion is not MIT-licensed.

Product behavior, verified claims and launch timing remain authoritative in the
[main warehouse repository](https://github.com/egemeny13/euroleague-analytics).
The current launch date is **2026-09-16**. This repository owns media production;
it does not independently redefine the product or its schedule.

---

# EuroLeague Analytics — 30-Second Launch Video (V2)

A clean, light-mode editorial launch video for **EuroLeague Analytics** built with [Remotion](https://www.remotion.dev/).

---

## 1. Quick Start & Preview

```bash
cd euroleague-analytics-launch

# Install dependencies
npm install

# Open interactive Remotion Studio in your browser
npm run dev
```

---

## 2. Rendering the Video

```bash
# Render and exact-trim the verified launch video
npm run build
```

### Video Specifications:
- **Duration**: 30.00 seconds (900 frames @ 30 fps)
- **Resolution**: 1920 &times; 1080 (1080p Full HD, 16:9)
- **Format**: H.264 MP4 with synchronized stereo audio
- **Palette**: Light editorial canvas (`#F8FAFC`), deep charcoal typography (`#0F172A`), and EuroLeague warm basketball orange (`#EA580C`)

---

## 3. What Changed in V2

1. **Light Editorial Palette**: Replaced the black background with an ultra-clean, modern light slate canvas (`#F8FAFC`) with high-contrast editorial typography and restrained EuroLeague orange accents.
2. **Interactive AI Conversation Scene (Heart of the Video)**:
   - Real-time typed question: *"How did Paris perform with TJ Shorts on vs. off the floor in E2024?"* with typing sound and blinking cursor.
   - Assistant *Thinking* phase with pulsing state and processing tone.
   - MCP tool execution indicator (`el_get_player_on_off` &bull; 2,488 possessions verified).
   - Hero answer presentation with camera zoom on the `+5.09` vs `-11.45` net rating split.
3. **Dynamic Motion & Continuous Camera Push-ins**: Eliminated the static feeling with smooth scale transitions, letter tracking, and camera momentum across all scenes.
4. **Enhanced Basketball & UI Sound Design**:
   - `typing.wav`: Mechanical keyboard typing burst
   - `thinking.wav`: Subtle electronic processing hum
   - `swish.wav`: Restrained basketball net swish
   - `impact.wav`: Hardwood sub-bass stat drops
   - `transition.wav`: Clean stereo transition sweeps
5. **Verified Repository Facts**:
   - **TJ Shorts On/Off Split**: ON `+5.09` vs OFF `-11.45` Net RTG (`+16.54` net swing, 2,488 possessions in E2024 &bull; *evaluation.xml #2*)
   - **732 Games Loaded** (330 in E2024 &bull; 402 in E2025)
   - **107,311 Reconstructed Possessions** (5 verified criteria)
   - **100.0% Final Score Reconciliation** (0 point discrepancies across all 732 games)

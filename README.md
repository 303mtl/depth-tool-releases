# 303 Tools — Releases

Public download & auto-update home for two macOS visual tools by **303mtl**.
This repo holds the finished, ready-to-run apps only — no source code.

---

## 303 Depth Tool (Kinect Depth Studio)

Turn **any video into an audio-reactive depth / point-cloud visual** — no Kinect
needed. Depth is estimated on your Mac's GPU by an AI model (Depth Anything V2),
so a flat clip becomes a 3D point cloud, LiDAR scan, thermal look, and more.

- **Drop in a video** → it's analysed once and cached.
- **10 looks** (KINECT RED, LIDAR WHITE, THERMAL SCAN, DEPTH EXPLOSION, RGB POINT
  CLOUD, INFRARED, DROP STREAK, CUTOUT BOUNCE, XBOX DEPTH, LIVE — KICK EXPLOSION).
- **Scenes** — save a whole look to a slot and recall it with one click.
- **Audio-reactive** — feed a live audio input and the visuals move with the music.
- **Live output to Resolume / OBS / TouchDesigner** via **Syphon** (local) and
  **NDI** (over the network, also Mac → Windows).
- **Export** H.264 / H.265 / ProRes 4444 (with alpha).

**Download:** [latest .dmg »](https://github.com/303mtl/depth-tool-releases/releases/latest)

---

## TYPOPLUGIN303

**Audio-reactive live typography** — type a word and it reacts to the music with
block, grid, slice, glitch and scroll modes. Live Syphon output for your VJ rig.

**Download:** [latest .dmg »](https://github.com/303mtl/depth-tool-releases/releases/tag/typo-v1.0.0)

---

## Install (first time only)

1. Open the `.dmg` and drag the app onto **Applications**.
2. Double-click it once — macOS blocks it (the app is not notarised by Apple).
3. **System Settings → Privacy & Security → "Open Anyway"**, then confirm.
   If it says *"is damaged"*, run once in Terminal:
   `xattr -dr com.apple.quarantine "/Applications/<App Name>.app"`

After that, **updates are one click**: when a new version is out, the app shows
*"Update available → Update now"* on launch and replaces itself.

**Requirements:** Apple Silicon Mac (M1 or newer), macOS 14 (Sonoma) or newer.
NDI output needs the free [NDI Tools](https://ndi.video/tools/) runtime installed.

---

## Credits

Thanks to **Giannis Veronis** ([@giannisveronis](https://github.com/giannisveronis))
for the Scenes idea and the NDI output, which were adapted into the Depth Tool.

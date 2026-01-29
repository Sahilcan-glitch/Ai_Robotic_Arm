# SO-ARM Robotic Arm (Full Setup + Teleop + Camera/Depth) 🤖

This repo documents my **end-to-end SO-ARM robotic arm build** — from **hardware setup + servo calibration** to **teleoperation** and **camera/depth-ready workflow** for future AI tasks (pick & place, object tracking, etc.).

> Goal: make it **reproducible** — if you have the same kit, you should be able to run it.

---

## What’s inside ✅
- ✅ Hardware + wiring checklist (power, USB, serial)
- ✅ Servo discovery + **calibration** (zeroing / limits)
- ✅ **Teleoperation** (leader → follower, or manual control)
- ✅ Camera setup (UVC) + notes for adding **depth**
- ✅ Troubleshooting for common serial/camera issues
- ✅ Clear project structure + scripts you can run

---

## Hardware (typical)
- SO-ARM (leader/follower) with servos (e.g., STS3215)
- Controller board + USB/serial adapter (depends on your kit)
- External power supply (important for stability)
- UVC camera (and optionally depth camera later)

---

## Software
- Python 3.10+ (recommended)
- Works best on macOS / Linux (Windows possible with COM port changes)

---

## Quickstart ⚡

### 1) Create environment
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt

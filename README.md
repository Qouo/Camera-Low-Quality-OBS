#  OBS Low-Res 144p Filter Plugin

##  Simulate bad video on purpose — to stick it to that micromanager

This OBS plugin applies a **retro low-quality video effect** to any source by:

- Downscaling it to **144p resolution**
- Capping it at **15–20 FPS**
- Upscaling it back to **1080p**, so it still fits your layout

This is for if you work from home and they require camera on, make it low quality! 
---

## Current Features

- Downscale any source to **144p**
- Limit framerate to ~15–20fps
- Output resolution stays at **1920×1080**
- Works as a **video filter** on any source
- Built using the OBS plugin SDK

---

## Installation

### Requirements

- OBS Studio (v27 or newer recommended)
- CMake
- C++ compiler (MSVC, GCC, Clang, etc.)
- Git (optional)

---

### Build From Source

```bash
git clone https://github.com/YOUR_USERNAME/obs-lowres-filter.git
cd obs-lowres-filter
mkdir build && cd build
cmake -DLIBOBS_INCLUDE_DIR="/path/to/obs/include" ..
cmake --build . --config Release

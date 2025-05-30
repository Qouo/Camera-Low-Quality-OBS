#  OBS Low-Res 144p Filter Plugin

##  Simulate bad video on purpose — to stick it to that micromanager

This OBS plugin applies a **retro low-quality video effect** to any source by:

- Downscaling it to **144p resolution**
- Capping it at **15–20 FPS**
- Upscaling it back to **1080p**, so it still fits your layout


## Current Features

- Downscale any source to **144p**
- Limit framerate to ~15–20fps
- Output resolution stays at **1920×1080**
- Works as a **video filter** on any source
- Built using the OBS plugin SDK

## Installation

### Requirements

- OBS Studio (v27 or newer recommended)
- CMake
- C++ compiler (MSVC, GCC, Clang, etc.)
- Git (optional)

### 🧱 Build From Source

###
bash
git clone https://github.com/YOUR_USERNAME/obs-lowres-filter.git
cd obs-lowres-filter
mkdir build && cd build
cmake -DLIBOBS_INCLUDE_DIR="/path/to/obs/include" ..
cmake --build . --config Release


Once built, copy the plugin binary to your OBS plugin folder:

- **Windows**: `C:\Program Files\obs-studio\obs-plugins\64bit`
- **macOS**: `/Library/Application Support/obs-studio/plugins`
- **Linux**: `~/.config/obs-studio/plugins`


##  How to Use

1. Open **OBS Studio**.
2. Add or select a video source (e.g. webcam, screen capture).
3. Click the **“Filters”** button below the source list.
4. Under **Effect Filters**, click the **+** icon.
5. Select **“Low-Res 144p Filter”** from the list.
6. The source will now appear heavily compressed and low resolution, while still fitting your 1080p scene.

>   You can combine this filter with audio effects for a fully scuffed look.



##  To-Do

Here are a few enhancements planned for this plugin:

- [ ] Add UI control to tweak output frame rate
- [ ] Simulate pixelation or block artifacts (like bad compression)
- [ ] Toggle dithering modes for extra retro effects
- [ ] Add settings panel for dynamic resolution/framerate
- [ ] Publish downloadable prebuilt binaries (Windows/macOS/Linux)
- [ ] Add demo video or GIF to this README
- [ ] Improve compatibility across multiple source types


##  Why Use This?

Use this plugin to:

- Fake a bad connection in a Zoom call
- Capture that bandicam feeling that you miss



## 👤 Author

- Created by Will Soteros 
- Built using the [OBS Studio Plugin API](https://github.com/obsproject/obs-studio)


##  License

MIT License

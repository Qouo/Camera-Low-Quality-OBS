# Camera-Low-Quality-OBS

📺 OBS Low-Res 144p Filter Plugin
🔧 Simulate bad video on purpose. For comedy, nostalgia, or... chaos.
This OBS plugin applies a retro low-quality video effect to any source by:

Downscaling it to 144p resolution

Capping it at 15–20 FPS

Upscaling it back to 1080p so it still fits your layout

Perfect for streamers, pranksters, or anyone who wants to look like they’re broadcasting from a potato 📦📡

🚀 Features
🎥 Downscale any source to 144p

🕒 Force framerate to ~15–20fps (optional frame skipping logic)

📈 Output maintains 1920×1080 canvas size

🖥️ Works as a filter on any video source

🧱 Built with OBS Studio's plugin SDK

📦 Installation
✅ Requirements
OBS Studio (v27+ recommended)

CMake

A C++ compiler

Git (optional)

💻 Build From Source (macOS/Linux/Windows)
bash
Copy
Edit
git clone https://github.com/YOUR_USERNAME/obs-lowres-filter.git
cd obs-lowres-filter
mkdir build && cd build
cmake -DLIBOBS_INCLUDE_DIR="/path/to/obs/include" ..
cmake --build . --config Release
⚠️ Replace /path/to/obs/include with the actual path to OBS headers on your system.

Copy the resulting .so, .dylib, or .dll file into OBS’s plugins directory:

Windows: C:\Program Files\obs-studio\obs-plugins\64bit

macOS: /Library/Application Support/obs-studio/plugins

Linux: ~/.config/obs-studio/plugins

🧪 How to Use
Launch OBS.

Add or select a video source (like your webcam).

Click the “Filters” button on that source.

Click the + under Effect Filters → Choose “Low-Res 144p Filter”

Watch your stream transform into glorious potato quality.

📋 To-Do
 Add FPS control slider

 Enable fake compression artifacts

 Toggle dithering modes

 Pre-built binaries for Windows/macOS/Linux

❓ Why?
Sometimes, high-quality isn't the vibe.

Whether you're doing a retro tech skit, looking for a fun transition effect, or trying to make your webcam look like a YouTube video from 2007 — this plugin's for you.

🧠 Credits
Created by YOUR NAME
Built using the OBS Studio Plugin API

📜 License
MIT License — use it, modify it, break it, fix it.

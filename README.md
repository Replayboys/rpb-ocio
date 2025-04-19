# 🎨 Replayboys OCIO Configuration

A streamlined and production-ready OpenColorIO configuration for modern color workflows.

## 🌟 Features

- 🎥 Optimized for ARRI workflows with LogC3/LogC4 support
- 🎬 Showgrade integration for show-specific looks
- 🖥️ Comprehensive display transforms for SDR and HDR
- 🎮 Blender-friendly with sRGB and Non-color spaces
- 🎯 Simplified for real-world production use

## 🚀 Quick Start

1. Place the config in your OCIO search path
2. Set `OCIO` environment variable to point to the config
3. Replace the showgrade LUTs with your show-specific versions

## 🎯 Supported Color Spaces

### Input Spaces
- ACES2065-1 (Reference)
- ARRI LogC3 (EI800)
- ARRI LogC4
- Linear Alexa Wide Gamut 3
- Linear Alexa Wide Gamut 4
- Blackmagic Design Film Generation 5
- Canon C-Log / C-Log2 / C-Log3
- GoPro Protune
- Panasonic V-Log
- RED Log3G10
- Sony S-Log3/S-Gamut3
- Sony S-Log3/S-Gamut3.Cine
- Sony S-Log3/S-Gamut3.Cine.Venice
- Linear S-Gamut3
- Linear S-Gamut3.Cine
- Linear S-Gamut3.Cine.Venice
- sRGB
- Linear Rec.709

### Working Spaces
- ACEScg
- ACEScc
- ACEScct
- Linear P3-D65
- Linear Rec.2020

### Display Spaces
- Rec.709 video
- Display P3
- Rec.2100-PQ (HDR)

## 🎨 View Transforms

### SDR Views
- Showgrade
- Replayboys Filmic
- ACES 2.0 SDR
- ACES 2.0 Filmic
- ACES 1.0 SDR
- Un-tone-mapped
- ARRI ALF2
- ARRI Reveal
- Khronos Neutral

### HDR Views
- Showgrade HDR 1000nit
- ACES 2.0 HDR 1000nit
- ACES 2.0 HDR P3Limited 1000nit
- ACES 2.0 Filmic HDR 1000nit
- ARRI ALF2 HDR 1000nit
- ARRI Reveal HDR 1000nit

## 🔧 Customization

### Showgrade Integration
1. Replace `luts/showgrade/showgrade_sdr.cube` for SDR
2. Replace `luts/showgrade/showgrade_hdr.cube` for HDR
3. The config will automatically use your show-specific LUTs

## 🛠️ Supported Applications

- Foundry Nuke
- Blender
- DaVinci Resolve
- Autodesk Flame
- SideFX Houdini
- And any other OCIO-compatible application

## 📁 Directory Structure

```
.
├── config.ocio
├── luts/
│   ├── showgrade/
│   │   ├── showgrade_sdr.cube
│   │   └── showgrade_hdr.cube
│   ├── ACES2/
│   ├── ARRI/
│   └── ...
└── README.md
```

## 🤝 Contributing

Feel free to submit issues and enhancement requests!

## 📜 License

This configuration is provided as-is for production use. Please respect the original authors' work and modifications.

## 👏 Credits

- Original configuration by Finn Jaeger @ Replayboys
- ARRI transforms by ARRI
- ACES transforms by AMPAS
- Additional contributions by the OCIO community
- Syncolor CTFs from Autodesk 
---

Made with ❤️ by Replayboys // Finn Jaeger

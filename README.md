# 🎨 Replayboys OCIO Configuration

A streamlined and production-ready OpenColorIO configuration for modern color workflows.

## 🌟 Features

- 🎥 Optimized for ARRI workflows with LogC3/LogC4 support
- 🎬 Showgrade integration for show-specific looks
- 🖥️ Comprehensive display transforms for SDR and HDR
- 🎮 Blender-friendly with sRGB and Non-color spaces
- 🎯 Simplified for real-world production use
- 📦 Extensive camera input support (ARRI, Sony, RED, Blackmagic, Canon, Panasonic)
- Support for ACES 2.0 (!!USING THE NOT-PERFECT LUT IMPLEMENTATION FROM PRV060!!) in OCIO 2.1 for backwards compatibility. (if anyone knows a better way LMK)

## 🚀 Quick Start

1. Clone or download this repository:
   ```bash
   git clone https://github.com/replayboys/rpb-ocio.git
   ```

2. Set up the OCIO environment:
   ```bash
   # Linux/macOS
   export OCIO=/path/to/rpb-ocio/config.ocio
   
   # Windows
   set OCIO=C:\path\to\rpb-ocio\config.ocio
   ```

3. Replace the showgrade LUTs with your show-specific versions:
   - Replace `luts/showgrade/showgrade_sdr.cube` for SDR
   - Replace `luts/showgrade/showgrade_hdr.cube` for HDR

## 🎯 Supported Color Spaces

### Input Spaces
- ACES2065-1 (Reference)
- ADX10 / ADX16
- ARRI LogC3 (EI800)
- ARRI LogC4
- Linear ARRI Wide Gamut 3
- Linear ARRI Wide Gamut 4
- Blackmagic Design Film Generation 5
- Linear BMD WideGamut Gen5
- DaVinci Intermediate WideGamut
- Linear DaVinci WideGamut
- Canon Log3 CinemaGamut D55
- Linear CinemaGamut D55
- Panasonic V-Log V-Gamut
- Linear V-Gamut
- RED Log3G10 WideGamutRGB
- Linear REDWideGamutRGB
- Sony S-Log3/S-Gamut3
- Sony S-Log3/S-Gamut3.Cine
- Sony S-Log3/S-Gamut3.Cine.Venice
- Linear S-Gamut3
- Linear S-Gamut3.Cine
- Linear Venice S-Gamut3
- Linear Venice S-Gamut3.Cine
- Camera Rec.709
- sRGB
- Linear Rec.709
- AppleLog

### Working Spaces
- ACEScg
- ACEScc
- ACEScct
- Linear P3-D65
- Linear Rec.2020

### SDR Displays
- Rec.1886 Rec.709 - Display
- Display P3 - Display

### HDR Displays
- Rec.2100-PQ - Display
- ST2084-P3-D65 - Display  

## 🎨 View Transforms

"Filmic" is a custom Film-emulation look made by Finn Jaeger

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
- ARRI Reveal HDR P3Limited 1000nit

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
│   │   ├── alf2/
│   │   └── reveal/
│   ├── khronos/
│   ├── replayboys/
│   └── shotluts/
└── README.md
```

## 📝 License

This configuration is provided as-is , development only

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 👏 Credits

- Original configuration by Finn Jaeger @ Replayboys
- Help with OCIO 2.0 by Doug Walker @ Autodesk
- ARRI transforms by ARRI
- ACES transforms by AMPAS
- Additional contributions by the OCIO community
- Shebanjah Klaasen for providing the AppleLog IDT as 1D LUT and matrix
---

Made with ❤️ by Replayboys // Finn Jaeger



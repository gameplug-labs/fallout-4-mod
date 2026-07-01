# GamePlug Fallout 4 Upscaler Mod

Adds FSR3, DLSS, XeSS, or DLAA upscaling and FSR3 frame generation to Fallout 4 using the GamePlug D3D11 layer. Improves image clarity and performance scaling while preserving the original game experience.

Enhance Fallout 4 with modern upscaling support through the GamePlug D3D11 layer. This mod injects FSR1/2/3, DLSS, XeSS3, or DLAA upscaling along with FSR3 frame generation into the game, allowing improved image reconstruction and better performance scaling at lower rendering resolutions while maintaining visual quality.

> [!NOTE]
> - Currently, changing the quality type directly in-game is not supported natively; by default, only Native AA or DLAA works.
> - You can now change the quality type by using the **F4SE Bridge Plugin**.

---

## Requirements

- **GPU Support:**
  - DirectX 11 compatible GPU (required)
  - RTX GPU (required for DLSS & NVIDIA Reflex)
  - DirectX 12 compatible GPU (required for XeSS3)
- **Settings:**
  - Disable in-game TAA (or any other settings causing image blur) for the best visual quality.
- **Compatibility:**
  - May be compatible with **ReShade**, though some lighting-related issues might occur.

---

## Features

- **Upscaling Support:** FSR1, FSR2, FSR3, DLSS, DLAA, XeSS3
- **Frame Generation:** FSR3 Frame Generation support
- **Tailored for Fallout 4:** Custom integration designed specifically for this game
- **Easy Injection:** D3D11-based lightweight DLL mod
- **In-Game Toggle:** Toggle the upscaler menu visibility using the `Ctrl + HOME` hotkey
- **Configuration:** Fully controllable via `upscaler_plugin.conf` (requires game restart to apply changes)

---

## Downloads

### Required for v1.1
- **Upscaler Plugin**: [upscaler-plugin-d3d11-d3d12](https://github.com/gameplug-labs/upscaler-plugin-d3d11-d3d12) (contains `upscaler_plugin.dll` and `upscaler_plugin.conf`)
- **F4SE (Fallout 4 Script Extender)**: [Nexus Mods](https://www.nexusmods.com/fallout4/mods/42147)
- **Address Library for F4SE Plugins**: [Nexus Mods](https://www.nexusmods.com/fallout4/mods/47327)
- **GamePlug Fallout 4 F4SE Bridge Plugin**

### Optional (Download required files for your preferred upscaling type)
- **FSR2 v2.2.1 files**: [FidelityFX FSR2 DX11 Releases](https://github.com/gameplug-labs/FidelityFX-FSR2-DX11/releases/tag/v2.2.1)
- **FSR3 v3.1.2 files**: [FidelityFX SDK Releases](https://github.com/gameplug-labs/FidelityFX-SDK/releases/tag/fsr3-v3.1.2) *(Required for Frame Generation)*
- **DLSS files**: [NVIDIA Streamline Releases](https://github.com/NVIDIA-RTX/Streamline/releases/tag/v2.11.1)
- **XeSS3 files**: [Intel XeSS Releases](https://github.com/intel/xess/releases/tag/v3.0.1)

---

## Installation

1. **Download the mod files.**
2. **Place the following files** into your Fallout 4 game executable directory:
   - `upscaler_plugin.dll`
   - `upscaler_plugin.conf`
   - `version.dll`
   - **Plus the DLL files corresponding to your chosen upscaler:**
     - **For FSR2:**
       - `ffx_fsr2_api_x64.dll`
       - `ffx_fsr2_api_dx11_x64.dll`
     - **For FSR3 Upscaling:**
       - `ffx_fsr3upscaler_x64.dll`
       - `ffx_backend_dx11_x64.dll`
     - **For FSR3 Frame Generation:**
       - `ffx_frameinterpolation_x64.dll`
       - `ffx_opticalflow_x64.dll`
     - **For DLSS:**
       - `sl.interposer.dll`
       - `sl.dlss.dll`
       - `sl.common.dll`
       - `nvngx_dlss.dll`
       - `sl.reflex.dll`
       - `sl.pcl.dll`
     - **For XeSS:**
       - `libxess.dll`
       - `libxess_dx11.dll` *(Optional - required for Intel Arc GPU only)*
3. **Launch the game.**
4. **Restart the game** after changing any settings (e.g., upscaler type, native, or quality mode).

---

## Framework

Powered by [GamePlug](https://github.com/gameplug-labs).

Join the [GamePlug Discord](https://discord.gg/TyyDD3C7wQ) for announcements, news, and new features!

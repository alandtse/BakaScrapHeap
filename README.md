# Baka ScrapHeap - Script Memory Limit Expander

A version independent F4SE plugin that expands the default size of ScrapHeap allocations.

- [Nexus](https://www.nexusmods.com/fallout4/mods/46340)
- [VR](https://www.nexusmods.com/fallout4/mods/85721)

## Requirements

- Any terminal of your choice (e.g., PowerShell)
- [Visual Studio Community 2022](https://visualstudio.microsoft.com/)
  - Desktop development with C++
- [CMake](https://cmake.org/)
  - Edit the `PATH` environment variable and add the cmake.exe install path as a new value
  - Instructions for finding and editing the `PATH` environment variable can be found [here](https://www.java.com/en/download/help/path.html)
- [Git](https://git-scm.com/downloads)
  - Edit the `PATH` environment variable and add the Git.exe install path as a new value
- [Vcpkg](https://github.com/microsoft/vcpkg)
  - Install vcpkg using the directions in vcpkg's [Quick Start Guide](https://github.com/microsoft/vcpkg#quick-start-windows)
  - After install, add a new environment variable named `VCPKG_ROOT` with the value as the path to the folder containing vcpkg

## User Requirements

- [Address Library for F4SE](https://www.nexusmods.com/fallout4/mods/47327)
  - Needed for SSE/AE
- [VR Address Library for F4SEVR](https://www.nexusmods.com/fallout4/mods/64879)
  - Needed for VR

## Register Visual Studio as a Generator

- Open `x64 Native Tools Command Prompt`
- Run `cmake`
- Close the cmd window

## Clone and Build

Open terminal (e.g., PowerShell) and run the following commands:

```ps
git clone https://github.com/alandtse/BakaScrapHeap.git --recursive
cd BakaScrapHeap
.\update-submodule.bat
.\make-sln-msvc.bat
.\build-msvc.bat
```

## License

[GPL-3.0-or-later](COPYING) WITH [Modding Exception AND GPL-3.0 Linking Exception (with Corresponding Source)](EXCEPTIONS).  
Specifically, the Modded Code is Fallout 4 (and its variants) and Modding Libraries include [F4SE/VR](https://f4se.silverlock.org/), [CommonlibF4](https://github.com/alandtse/CommonLibF4) (and variants), and [DKUtil](https://github.com/gottyduke/DKUtil).

## Credits

Forked from https://github.com/shad0wshayd3-FO4/BakaScrapHeap

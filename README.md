# Moviola Exporter - GPL Compliance Package

This repository provides the source code and documentation necessary to comply with the GNU General Public License (GPL) for components used in the Moviola Video Editor VR app's export system.

## Why this exists

The Moviola export system integrates with `libx264` (a GPLv3 library) via the `mobile-ffmpeg-full-gpl-4.4.LTS.aar` package. To comply with GPL terms, we are publishing:

- The full source code related to the export logic
- The binaries and bridge used to integrate FFmpeg
- Licensing and build instructions

This repository **does not include the full Moviola app**, UI, scenes, assets, or commercial features.

## Contents

- `FFmpegHandler.cs` and related C# export scripts
- `FFmpegUnityBind2` native bridge + `.aar` binary
- `mobile-ffmpeg-full-gpl-4.4.LTS.aar` (used at runtime)
- `LICENSE` (GPLv3)
- `build_instructions.md` for rebuilding the export logic

## FFmpeg Notice

This project includes a binary dependency (`mobile-ffmpeg-full-gpl-4.4.LTS.aar`) built from:
[https://github.com/tanersener/mobile-ffmpeg/tree/v4.4.LTS](https://github.com/tanersener/mobile-ffmpeg/releases/tag/v4.4.LTS)

That package statically links `libx264`, a GPLv3 component.

## Contact

If you are the maintainer or rights holder of any third-party library included here and believe attribution or source code is incomplete, please [open an issue](https://github.com/kevinagnes/moviola-exporter-gpl-source/issues) or email contact@xr.dev.br.

---

This repository is published in good faith to fulfill all obligations of GPL-covered components.

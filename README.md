# HandBrake-SVT-AV1-Tritium
### Purpose of the project
This project contains the patches needed to replace SVT-AV1 with SVT-AV1-Tritium inside HandBrake.\
SVT-AV1-Tritium is a fork of SVT-AV1-HDR that incorporates features from other forks, such as SVT-AV1-PSYEX and SVT-AV1-Essential. Most notably, SVT-AV1-Tritium includes scene detection and auto-tiling from SVT-AV1-Essential.\
Scene detection and auto-tiling are enabled by default, other than that, the default settings are the same as SVT-AV1-HDR.\
In addition, using GitHub Actions, nightly build of patched executables will be released.
### Instructions to patch/build
* Run ```patch.sh``` on linux. The script will patch the previously cloned HandBrake repo. If you want to also clone it you can use ```--clone``` argument.
* Compile for the desired platform using the commands provided on the HandBrake wiki ([BSD](https://handbrake.fr/docs/en/latest/developer/build-bsd.html), [Linux](https://handbrake.fr/docs/en/latest/developer/build-linux.html), [Mac](https://handbrake.fr/docs/en/latest/developer/build-mac.html), [Windows](https://handbrake.fr/docs/en/latest/developer/build-windows.html))
### Downloads and Build Status
| Operating System  | Download        | Build Status *1 |
| ----------------- | --------------- | ------------- |
| Windows           | [Download](https://github.com/Uranite/HandBrake-SVT-AV1-Tritium/releases/tag/win) | [![Windows Build](https://github.com/Uranite/HandBrake-SVT-AV1-Tritium/actions/workflows/nightly-win.yml/badge.svg)](https://github.com/Uranite/HandBrake-SVT-AV1-Tritium/actions/workflows/nightly-win.yml)  |
| macOS             | [Download](https://github.com/Uranite/HandBrake-SVT-AV1-Tritium/releases/tag/mac) | [![macOS build](https://github.com/Uranite/HandBrake-SVT-AV1-Tritium/actions/workflows/nightly-mac.yml/badge.svg)](https://github.com/Uranite/HandBrake-SVT-AV1-Tritium/actions/workflows/nightly-mac.yml)  |
| Linux (Flatpak)   | [Download](https://github.com/Uranite/HandBrake-SVT-AV1-Tritium/releases/tag/flatpak) | [![Flatpak Build](https://github.com/Uranite/HandBrake-SVT-AV1-Tritium/actions/workflows/nightly-flatpak.yml/badge.svg)](https://github.com/Uranite/HandBrake-SVT-AV1-Tritium/actions/workflows/nightly-flatpak.yml) |
| Ubuntu            | [Download](https://github.com/Uranite/HandBrake-SVT-AV1-Tritium/releases/tag/ubuntu) | [![Flatpak Build](https://github.com/Uranite/HandBrake-SVT-AV1-Tritium/actions/workflows/nightly-ubuntu.yml/badge.svg)](https://github.com/Uranite/HandBrake-SVT-AV1-Tritium/actions/workflows/nightly-ubuntu.yml) |
| Arch Linux        | [Download](https://github.com/Uranite/HandBrake-SVT-AV1-Tritium/releases/tag/arch) | [![Flatpak Build](https://github.com/Uranite/HandBrake-SVT-AV1-Tritium/actions/workflows/nightly-arch.yml/badge.svg)](https://github.com/Uranite/HandBrake-SVT-AV1-Tritium/actions/workflows/nightly-arch.yml) |

*1 Please note that if a build is marked as failed, previous builds may still be available for download!
### Testing
I can currently only test the custom build on Windows. Help for testing on other platforms would be helpful.
### Special thanks
A special thanks to [vincejv (Docker container for HandBrake)](https://github.com/vincejv/docker-handbrake) from which I took inspiration for some patches.


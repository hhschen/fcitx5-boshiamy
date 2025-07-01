# fcitx5-boshiamy

- [English README](README.en.md)
- [中文說明](README.zh_TW.md)

## Introduction

`fcitx5-boshiamy` is a standalone module providing Boshiamy input method support for the Fcitx5 input framework. This project extracts the Boshiamy table from the original [fcitx5-table-extra](https://github.com/fcitx/fcitx5-table-extra) repository, enabling independent usage.

## Requirements

- Runtime dependencies: `fcitx5-im`, `fcitx5-chinese-addons`, `libime`
- Build dependencies: `cmake`, `extra-cmake-modules`, `boost`

## Build and Installation

```bash
mkdir build
cd build
cmake .. -DCMAKE_INSTALL_PREFIX=<fcitx's prefix>
cmake --build .
cmake --install .  # Root privileges may be required
```

## Overview

This project is a standalone extraction of the Boshiamy table from the original [fcitx5-table-extra](https://github.com/fcitx/fcitx5-table-extra) repository. It is intended to provide Boshiamy input support independently.

## Disclaimer

This repository is **not affiliated** with the original fcitx5-table-extra project or the Fcitx team. It is a personal extraction and modification for convenience.

All original copyrights and licenses apply to the code and data originating from fcitx5-table-extra.

The code of this package are released under GPLv3 or later.

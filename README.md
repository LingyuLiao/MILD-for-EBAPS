# MILD: Multi-Illumination Low-Light EBAPS Dataset

## Overview

MILD is a multi-illumination low-light image dataset acquired using an Electron-Bombarded Active Pixel Sensor (EBAPS). It contains paired images captured under different illumination conditions, providing real-world data for low-light image denoising, enhancement, and related research.


## Dataset Download

The current version of MILD is available through Baidu Netdisk:

- **Download Link:** https://pan.baidu.com/s/1zS0lPggZpAfaX-iJRED-Cw?pwd=nvxz
- **Extraction Code:** `nvxz`

## Dataset Structure

All scene folders are stored directly under the `data/` directory and named according to their scene IDs.

Each scene contains seven images:
- **6 low-light images** captured at different illumination levels.
- **1 reference image (GT)** captured under normal exposure conditions.

The directory structure is organized as follows:

```text
data/
├── 1/
│   ├── 1-1E-2.JPG
│   ├── 1-2E-3.JPG
│   ├── 1-4E-2.JPG
│   ├── 1-5E-5.JPG
│   ├── 1-7E-4.JPG
│   ├── 1-9E-5.JPG
│   └── 1-GT.JPG
├── 2/
│   └── ...
├── 3/
│   └── ...
└── ...
```

### File Naming Convention

Low-light images follow the naming format:

`{SceneID}-{Illumination}.JPG`

The illumination level is expressed in scientific notation (in lux). For example:

- `1-1E-2.JPG`: Scene 1 captured at 1 × 10⁻² lx.
- `1-5E-5.JPG`: Scene 1 captured at 5 × 10⁻⁵ lx.
- `1-GT.JPG`: Normally exposed reference image for Scene 1.

The six low-light illumination levels are:

**4 × 10⁻², 1 × 10⁻², 2 × 10⁻³, 7 × 10⁻⁴, 9 × 10⁻⁵, and 5 × 10⁻⁵ lx.**

## Future Updates

This is an initial release containing 500 scenes in JPG format.

The complete MILD dataset, including additional scenes and RAW-format images, is currently being organized and will be released in future updates.

Please stay tuned to this repository for further updates.

## Contact

For questions or inquiries regarding the dataset, please feel free to open an issue in this repository.

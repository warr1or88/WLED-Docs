---
title: Fork Comparison
hide:
  # - navigation
  # - toc
---

## What are the differences between WLED SR, upstream AC WLED, and MoonModules fork?


Feature | [WLED SR 0.13](https://github.com/atuline/WLED/tree/dev) | [MoonModules WLED 0.14](https://github.com/MoonModules/WLED/tree/mdev) | [Upstream WLED 0.14](https://github.com/Aircoookie/WLED) 

| Type | Voltage | Comments |
|---|---|---|
SK6812 | 5v | RGBW
WS2811 | 5v | usually found in IP68 sealed 12mm pixel strings
WS2812B | 5v |

Feature | MM | Upstream | AC
|---|---|---|---|
0.14 architecture | No | Yes (upstream frequently merged) | Yes

| Feature | MM | Upstream | AC |
|---|---|---|---|
0.14 architecture | No | Yes (upstream frequently merged) | Yes
Usermods have own pages in main config menu | Audio Reactive only | Yes | No
Segments 2D aware | No (XY calculated, mirror not working) | Yes | Yes
Audio reactive | Core | Usermod | Usermod
Microphone Profiles | No | Yes | No | 
Audio dynamics limiter | No | Yes | Yes
High Definition audio analysis, 32 channel GEQ | No |  Yes (WIP) for ESP32 and ESP32-S3 | No
Custom Effects | Yes | Yes as a usermod! | No
Effect ID's | 0.13 compatible | 0.13 compatible (recommended!) | Changed, old SR presets will not work.
Expand 1D effects | No | Yes (+ Circles and Block) | Yes
Extended hw info | basic | Yes | No
JSON Mapping on 1D effects | No | Yes | No
Games usermod (3D to 2D, gyro) | No | Yes (WIP) | No
Weather usermod (syncing internet data) | No | Yes (WIP) | No
HB effects | Fully supported | 80% supported (WIP) | Not supported
classic ESP32 | Yes | Yes | Yes
ESP32-S3 | No | Yes | Experimental
ESP32-S2 and ESP32-C3 | No | Experimental | Experimental
ESP8266 | No | No | Yes but no Audio Reactive for 8266
Ledmaps in presets | Yes | No (wait for upstream fix) | No

# Jetson Orin Baseboard

Copyright (c) 2022-2024 [Antmicro](https://www.antmicro.com)

[![image](https://img.shields.io/badge/View%20on-Antmicro%20Open%20Hardware%20Portal-332d37?style=flat-square)](https://openhardware.antmicro.com/boards/jetson-orin-baseboard)
[![image](https://img.shields.io/badge/View%20on-Antmicro%20Open%20Source%20Portal-332d37?style=flat-square)](https://opensource.antmicro.com/projects/jetson-orin-baseboard)

![](img/jetson-orin-baseboard-photo.png)

## Overview

This project contains open hardware design files for a baseboard supporting NVIDIA Jetson Orin Nano and Jetson Orin NX System on Modules (SoMs).
The board break-routes the typical IO interfaces from the SoM.
Additionally, it exposes an expansion connector which allows it to be integrated with external processing modules using PCIe or low-speed interfaces.

The design files were preapared in KiCad 7.x.

## Key features

* Two USB PD ports
* DC Power connector
* MIPI CSI-2 interfaces on 50-pin connectors with configurable lane mapping
* Micro HDMI connector
* USB-C 10 Gbps with USB PD and DP
* USB-C 10 Gbps
* USB-C UART with USB PD
* M.2 key M
* M.2 key E
* 1Gb Ethernet with PoE
* Custom expansion connector
* RTC battery backup

## Project structure

The main directory contains KiCad PCB project files, a LICENSE, and a README.
The remaining files are stored in the following directories:

* `img` - contains graphics for this README
* `doc` - contains schematics in pdf form
* `assets` - contains visual assets for showcasing this design on [Open Hardware Portal](https://openhardware.antmicro.com/boards/jetson-orin-baseboard/?tab=features&view=top-ortho).

The board exposes MIPI CSI-2 interfaces using unified 50-pin connectors that are electrically compatible with a variety of video accessories created by Antmicro:

* [SDI-MIPI Video converter](https://github.com/antmicro/sdi-mipi-video-converter)
* [FRAMOS camera adapter](https://github.com/antmicro/framos-csi-adapter)
* [Allied Vision Alvium Camera Adapter](https://github.com/antmicro/alvium-flexible-csi-adapter)
* [HDMI-MIPI bridge](https://github.com/antmicro/hdmi-mipi-bridge)
* [OV9281 Dual camera board](https://github.com/antmicro/ov9281-camera-board)

## Licensing

This project is published under the [Apache-2.0](LICENSE) license.


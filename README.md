# LimeNET-Micro

![LimeNET-Micro board](/images/LimeNET-Micro_722w.jpg)

The [LimeNET Micro](https://www.crowdsupply.com/lime-micro/limenet-micro) makes deploying wireless networks more accessible than ever before, by extending the LimeNET line of integrated hardware solutions via an ultra-low cost platform that is capable of supporting narrowband systems, such as GSM and IoT wireless standards, in a stand-alone configuration.

* **RF transceiver:** Lime Microsystems LMS7002M
* **FPGA Features** 
  * Intel Altera MAX 10 (10M16SAU169C8G)
  * 169-pin FBGA package
  * 16K LEs
  * 549 KB M9K memory
  * 2,368 KB user flash memory
  * 4 x fractional phase locked loops (PLLs)
  * 45 x 18x18-bit multipliers
  * 130 x general purpose input/output (GPIO)
  * Single supply voltage
  * Flash feature
  * FPGA configuration via JTAG
* **GNSS module:** u-blox NEO-M8Q-0-10
  * Supports BeiDou, Galileo, GLONASS, GPS / QZSS
  * Able to concurrently receive up to three GNSS
  * –167 dBm navigation sensitivity
* **EEPROM memory:** 2 x 128 KB for RF transceiver MCU firmware and data
* **Flash memory:** 1 x 4 MB flash memory for data
* **General user inputs/outputs:**
  * 5 x dual color (red + green) LED
  * 8 x FPGA GPIO pinheader (3.3 V)
  * 4 x FPGA switches
  * 1 x buzzer
* **Connectivity:**
  * 2 x coaxial RF (SMA) connectors (each can be switched between high and low frequency bands)
  * SMA connector for external clock source in
  * SMA connector for clock source out
  * SMA connector for GNSS antenna
  * Raspberry Pi Touch Screen Display Connector (ribbon cable)
  * Raspberry Pi Camera (ribbon cable)
  * HDMI connector
  * 2 x USB 2.0 ports
  * 3.5 mm audio out (Raspberry Pi Compute Module)
  * FPGA GPIO headers
  * FPGA JTAG connector
  * RJ45 connector for Ethernet and IEEE 802.3 active Power-over-Ethernet (PoE)
  * DDR2 SODIMM connector - only usable for Raspberry Pi Compute Module 3 (or Lite)
  * MicroSD slot for RPi Compute Module storage
  * Barrel connector for 5 V DC power
  * Micro-USB for USB boot of Compute Module
* **Clock system:**
  * 30.72 MHz OCXO: Rakon U7475LF
  * GPS disciplined for high frequency accuracy and stability
  * External clock input via SMA connector
  * Clock output via SMA connector
* **Board dimensions:** 125 mm x 65 mm

## Contents

The directory structure is as follows:

      hardware/<version>/
          Libraries/             - Component Libraries
          OutputJobs/            - Output jobs
          PCB/                   - PCB design
          Project Outputs/       - BOM, rule check reports, Gerbers, pick & place files, PDFs
          Schematics/            - Schematic diagrams

## Licensing

The hardware designs are licensed under a Creative Commons Attribution 3.0 Unported licence.

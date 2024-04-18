# Dual Band ADS-B Reciever Enclosure

This project provides an enclosure for a [SAWbird+ ADS-B LNA & Filter](https://www.nooelec.com/store/sdr/sdr-addons/sawbird/sawbird-plus-adsb.html), an [Anker USB-C Hub](https://www.anker.com/products/a8356), and two [Nooelec NESDR Nano 3](https://www.nooelec.com/store/sdr/sdr-receivers/nesdr-nano-three.html) SDRs. A 40x10mm fan is also required, I used this [Noctua](https://noctua.at/en/nf-a4x10-flx) fan.

[Reference Photo Goes Here]

# Usage & Implementation

Contrary to other SDR-based enclosure projects, this enclosure is not intended to also house the device which does the demodulation and processing of the received ADS-B data.

The enclosure is intended to be used by plugging the USB-C cable from the hub directly into a device that can run the associated software package. The software repository includes support for Windows and Linux hosts.

# Software

This enclosure can be used as-is with any applications that support RTLSDRs. Otherwise, the software repository for this project includes a NixOS live iso that runs dump1090, dump978, and tar1090 for visualization. There is an included runner program that automatically hosts the iso with qemu.
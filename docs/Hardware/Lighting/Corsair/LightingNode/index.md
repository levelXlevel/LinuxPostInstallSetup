# Corsair Lighting Node Core

[Product Page](https://www.corsair.com/ca/de/Kategorien/Produkte/Zubeh%C3%B6r-%7C-Teile/CORSAIR-LINK/iCUE-Lighting-Node-CORE-Digital-Fan-RGB-Lighting-Controller/p/CL-8930009)

## UDEV

File: `/etc/udev/rules.d/99-corsair-lighting-node-core-rgb.rules`

```
SUBSYSTEM=="usb", ATTR{idVendor}=="1b1c", ATTR{idProduct}=="0c1a", GROUP="plugdev", MODE="0666"
```

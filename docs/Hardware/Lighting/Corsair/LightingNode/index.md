# Corsair Lighting Node Core

[Website]()

## UDEV

File: `/etc/udev/rules.d/99-corsair-lighting-node-core-rgb.rules`

```
SUBSYSTEM=="usb", ATTR{idVendor}=="1b1c", ATTR{idProduct}=="0c1a", GROUP="plugdev", MODE="0666"
```

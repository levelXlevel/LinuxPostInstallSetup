# Corsair M65 PRO RGB Mouse

[Product Page](https://www.corsair.com/us/en/Categories/Products/Gaming-Mice/FPS-Fast-Action-Mice/M65-RGB-ULTRA-Tunable-FPS-Gaming-Mouse/p/CH-9309411-NA2)

## UDEV

File: `/etc/udev/rules.d/99-corsair-m65-rgb.rules`

```
SUBSYSTEM=="usb", ATTR{idVendor}=="1b1c", ATTR{idProduct}=="1b2e", GROUP="plugdev", MODE="0666"
```

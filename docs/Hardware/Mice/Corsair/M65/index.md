# Corsair M65 PRO RGB Mouse

[Website]()

## UDEV

File: `/etc/udev/rules.d/99-corsair-m65-rgb.rules`

```
SUBSYSTEM=="usb", ATTR{idVendor}=="1b1c", ATTR{idProduct}=="1b2e", GROUP="plugdev", MODE="0666"
```

99-corsair-lighting-node-core-rgb.rules

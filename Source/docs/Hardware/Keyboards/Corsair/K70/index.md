# Corsair K70 RGB Mechanical Keyboard

[Website]()

## UDEV

File: `/etc/udev/rules.d/99-corsair-k70-rgb.rules`

```
SUBSYSTEM=="usb", ATTR{idVendor}=="1b1c", ATTR{idProduct}=="1b49", GROUP="plugdev", MODE="0666"
```

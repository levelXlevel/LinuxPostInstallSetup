# Corsair K70 RGB Mechanical Keyboard

[Product Page](https://www.corsair.com/us/en/k70-rgb-gaming-keyboard)

## UDEV

File: `/etc/udev/rules.d/99-corsair-k70-rgb.rules`

```
SUBSYSTEM=="usb", ATTR{idVendor}=="1b1c", ATTR{idProduct}=="1b49", GROUP="plugdev", MODE="0666"
```

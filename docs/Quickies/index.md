# Quickies

## Reload UDEV rules

> udevadm control --reload-rules && udevadm trigger

## Check for failed _systemd_ service

> sudo systemctl --failed

## Check for errors in logfiles

> sudo journalctl -p 3 -xb

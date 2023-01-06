# Fan Control

- Modify GRUB: `/etc/default/grub`
- Add the following to the Linux default command line parameter.
- The (...) dots are place holder for what will likely be there, don't remove what's already there, just add the parameter to the end.

```
GRUB_CMDLINE_LINUX_DEFAULT= ...
```

```
GRUB_CMDLINE_LINUX_DEFAULT= ... acpi_enforce_resources=lax
```

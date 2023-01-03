# CPUPower

## Description

Allows setting CPU power & Performance profiles.

## Discussion

- There is no need to setup the systemd unit (boot time). Especially if you are the sole user.
- Install CPUPower_Gui and let the user setup the profile as needed.
- Install global profiles so all users have access to them.

## Profiles

### Path

Global Profile Path: `/etc/cpupower_gui.d/`
User Profile Path: `~/.config/cpupower_gui/`

### Filenames

&lt;anyname&gt;.profile

I'd strongly recommend naming the file similarly to the intended profile name. The use of spaces is in the filename and profilename are also discouraged, especially if this is your first time.

## Examples

### Conservative

Config File: `/etc/cpupower_gui.d/Conservative.profile`

```
# name: Conservative

# CPU   Min Max Governor    Online
0-7 800 4000    conservative    True
```

### Powersave

Config File: `/etc/cpupower_gui.d/Powersave.profile`

```
# name: Powersave

# CPU   Min Max Governor    Online
0-7 1200    3600    powersave   True
```

## Boot Time

If you'd still like to setup the service to start at boot time, go on a head. I'd suggest configuring the service first before doing so or just restart it as needed as you make changes.

### Configure

Global Config File: `/etc/cpupower_gui.conf`
User Config File: `~/.config/cpupower_gui/00-cpg.conf`

N.B. This example assumes you have created the conservative profile.

```
[Profile]
profile = Conservative

[GUI]
allcpus_default = True
tick_marks_enabled = True
frequency_ticks = True
energy_pref_per_cpu = False
```

### Enable

```
sudo systemctl enable --now cpupower
```

# Ananicy

## Description

**AN**other **A**uto **NIC**e

A tool for controlling the priority of applications.

## Observation

Ananicy was installed & started by default, but it was missing _schedtool_ & _schedtoold_ which is used for controlling _ananicy_.

## Rules

Path: `/etc/ananicy.d/00-default/`

This is where you can find the predefined rules where were installed by default.

## Setup

### Install

Use you're prefered package manager to install _schedtool_ & _schedtoold_

> yay -S --noconfirm schedtool schedtoold

### Enable

> sudo systemctl enable --now schedtoold

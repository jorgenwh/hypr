# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a Hyprland configuration directory for a dual-monitor desktop setup. Hyprland is a dynamic tiling Wayland compositor.

## Files

- `hyprland.conf` - Main Hyprland compositor configuration (monitors, keybindings, appearance, window rules)
- `hyprlock.conf` - Lock screen configuration for hyprlock

## Key Configuration Details

**Monitors**: Dual-monitor setup with DP-1 (3440x1440@100Hz, ultrawide) as primary and HDMI-A-1 (2560x1440@144Hz) as secondary.

**Main Modifier**: ALT key (i3-style bindings)

**Key Bindings Pattern**:
- `$mainMod` (ALT) + key for actions (Q=kill, D=terminal, F=fullscreen, A=menu)
- `$mainMod` + SHIFT + key for window operations (move window, reload config)
- Vim-style navigation with H/J/K/L for focus and window movement
- Resize mode entered with ALT+R, uses H/J/K/L or arrows

**Workspaces**: 1-10 on main monitor (DP-1), with dedicated workspaces for Spotify (11/Z), Discord (12/X), Slack (13/C).

**Default Applications**:
- Terminal: kitty
- File manager: dolphin
- Launcher: wofi

## Testing Changes

Reload configuration with `hyprctl reload` or the keybind ALT+SHIFT+C.

## Documentation

- Hyprland wiki: https://wiki.hypr.land/
- Configuration reference: https://wiki.hypr.land/Configuring/
- Update the CLAUDE.md file when changing the hypr configuration.
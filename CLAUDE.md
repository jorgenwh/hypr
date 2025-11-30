# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a Hyprland configuration directory for a dual-monitor desktop setup. Hyprland is a dynamic tiling Wayland compositor.

## Files

- `hyprland.conf` - Main compositor configuration (monitors, keybindings, appearance, window rules)
- `hyprlock.conf` - Lock screen configuration for hyprlock
- `hyprpaper.conf` - Wallpaper configuration (uses moon.png)

## Key Configuration Details

**Monitors**: Dual-monitor setup with DP-1 (3440x1440@100Hz, ultrawide) as primary and HDMI-A-1 (2560x1440@144Hz) as secondary.

**Layout**: Master layout with 50% master factor, new windows spawn as slaves.

**Input**: Norwegian keyboard layout (`kb_layout = no`), fast key repeat (135ms delay, 50 rate).

**Main Modifier**: ALT key (i3-style bindings)

**Key Bindings Pattern**:
- `$mainMod` (ALT) + key for actions (Q=kill, D=terminal, F=fullscreen, A=menu, S=chrome, E=play-pause, P=screenshot)
- `$mainMod` + SHIFT + key for window operations (move window, reload config, exit)
- SUPER+L for lock screen
- Vim-style navigation with H/J/K/L for focus and window movement
- Resize mode entered with ALT+R, uses H/J/K/L or arrows, exit with Return/Escape/ALT+R

**Workspaces**: 1-9 on DP-1, workspace 10 on HDMI-A-1, with dedicated workspaces for Spotify (11/Z), Discord (12/X), Slack (13/C) on DP-1.

**Autostart**: waybar, nm-applet, and silent launches of Spotify, Discord, Slack on their respective workspaces.

**Default Applications**:
- Terminal: kitty
- File manager: dolphin
- Launcher: wofi
- Browser: google-chrome-stable

## Testing Changes

Reload configuration with `hyprctl reload` or the keybind ALT+SHIFT+C.

## Documentation

- Hyprland wiki: https://wiki.hypr.land/
- Configuration reference: https://wiki.hypr.land/Configuring/
- Update the CLAUDE.md file when changing the hypr configuration.
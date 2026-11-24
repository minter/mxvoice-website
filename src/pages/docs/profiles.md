---
title: Profiles
subtitle: Separate setups for different performers, teams, or venues
layout: ../../layouts/Docs.astro
image: /docs/profile-launcher.png
---

## Overview

Profiles let you maintain completely separate setups within Mx. Voice. Each profile has its own [shows](/docs/shows/) (saved hotkey and holding tank layouts) and display preferences. This is useful when multiple performers share a computer.

If you just want different layouts for different venues, teams, or formats, you don't need separate profiles — save each layout as a show within one profile.

## The Profile Launcher

When you start Mx. Voice, the Profile Launcher appears. It shows a list of all available profiles. Select one and click **Open**, or double-click a profile to open it directly.

<img src="/docs/profile-launcher.png" alt="Profile Launcher" width="420" />

You can search for profiles by name or description using the search field in the launcher.

## Default Profile

On first launch, a **Default User** profile is created automatically. It appears at the top of the profile list and cannot be deleted. If you're the only person using the computer, you can use this profile for everything.

## Creating a Profile

1. Click **New profile** in the launcher, or choose **Profile → New Profile…** in the menu bar.
2. Enter a **Profile Name** (required, up to 50 characters). Letters, numbers, spaces, hyphens, and underscores are allowed.
3. Optionally enter a **Description** (e.g., "Friday night show at Club XYZ").
4. Click **Create profile**.

<img src="/docs/new-profile.png" alt="New Profile" width="500" />

New profiles start with default preferences and empty hotkey and holding tank tabs. To bring in a layout from another profile, use **Shows → Import Show from Another Profile…**. Profile names must be unique.

## Switching Profiles

To switch to a different profile, go to **Profile → Switch Profile…** in the menu bar. The profile list opens right in the window, without restarting the app. Your current profile is grayed out, and **Esc** takes you back.

<img src="/docs/switch-profile.png" alt="Switch Profile" width="500" />

Switching profiles doesn't save the loaded show. If you've made changes you want to keep, use **Shows → Save** first.

## Deleting a Profile

Click the delete button next to a profile in the launcher. The Default User profile and the last remaining profile cannot be deleted.

> **Warning:** Deleting a profile permanently removes all of its shows and preferences. Your song database and audio files are not affected.

## What's Isolated per Profile

Each profile maintains its own:

- **Shows** — each one a saved layout of hotkey assignments (all 5 tabs, F1–F12 each) and holding tank lists (all 5 tabs)
- **Display preferences** — screen mode (light/dark/auto), fade-out duration, column order
- **Prerelease updates** — whether beta versions are offered
- **Window state** — window size and position

## What's Shared Across Profiles

All profiles share:

- **Song database** — all profiles search the same library of songs. Adding or removing songs affects all profiles.
- **Directory settings** — audio files directory, database location, and hotkey/holding tank file directory.
- **Debug logging** — the logging toggle is global.

## Where Profiles Are Stored

Profile data is stored in your system's application data directory:

| Platform | Location |
| --- | --- |
| **macOS** | `~/Library/Application Support/Mx. Voice/` |
| **Windows** | `%APPDATA%\Mx. Voice\` |
| **Linux** | `~/.config/Mx. Voice/` |

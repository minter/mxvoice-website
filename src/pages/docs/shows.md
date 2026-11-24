---
title: Shows
subtitle: Save hotkey and holding tank layouts, and switch between them
layout: ../../layouts/Docs.astro
---

## Overview

Starting in version 4.4, your hotkeys and holding tank are kept as a **show**. A show is a saved layout: every hotkey tab, every holding tank tab, and the tab names. Each profile can have as many shows as you like — one per venue, team, or format — and you switch between them from the **Shows** menu.

The header at the top of the window shows your profile and the show that's loaded.

## Upgrading from an Earlier Version

The first time you open a profile in 4.4, the hotkeys and holding tank you had become a show named **Default Show**. Nothing is lost, and you can rename it.

> **Important:** Before 4.4, Mx. Voice saved your hotkeys and holding tank automatically when you quit. It no longer does. Changes made during a show are kept **only if you save them** with **Shows → Save**.

## Saving a Show

Changes you make to the hotkeys and holding tank stay on screen until you save or discard them.

| Menu item | What it does |
| --- | --- |
| **Shows → Save** | Updates the loaded show with the layout on screen. |
| **Shows → Save As…** | Saves the layout on screen as a new show. |
| **Shows → Revert to Saved…** | Puts the show back as you last saved it, dropping changes made since. Available only while there are unsaved changes. |

A **dot** after the show name in the header means the layout on screen has unsaved changes.

Quitting or switching profiles doesn't save the show. Next time, it opens as you last saved it. This means you can rearrange things freely during a performance and start the next one from your prepared layout.

## Switching Shows

Every show in the current profile is listed at the top of the **Shows** menu. Choose one to load it. If the layout on screen has unsaved changes, Mx. Voice asks whether to save them first.

## Renaming, Coloring, and Deleting

These act on the show that's loaded. To change a different show, switch to it first.

- **Shows → Rename** — Give the show a new name.
- **Shows → Color** — Give the show an accent color: Teal, Blue, Purple, Pink, Coral, Amber, or Green. The color appears behind the panels, under the active tab, and around the show name, so you can see at a glance which show is loaded. It saves right away. Choose **None** to remove it.
- **Shows → Delete** — Delete the show.

## Importing a Show from Another Profile

**Shows → Import Show from Another Profile…** copies a saved show from another profile on this computer. The copy is yours to change — the original is not affected. If you have unsaved changes, Mx. Voice asks whether to save them first.

## Tab Files

A show holds all of your tabs. To keep or share a single tab — a pre-show playlist, or a standard set of drops — save it as a tab file. Open the **⋯** menu at the end of a tab row, or right-click a tab:

- **Save Tab to File…** — Saves that one tab to a file.
- **Load Tab from File…** — Loads a file into that tab. If the tab already has songs, Mx. Voice asks first.

Tab files are the same **.mrv** (hotkey) and **.hld** (holding tank) files that earlier versions use. If you kept a show in one of those files, load it onto a tab and then use **Shows → Save** or **Save As…**.

The Hotkeys menu, its **Cmd/Ctrl+O** and **Cmd/Ctrl+S** shortcuts, and the folder and save icons from earlier versions are gone.

## Played Counts

A **▶ count** appears next to every track you've played tonight, in the hotkeys, the holding tank, and the search results. You can see what's been used without removing it.

- **Clear one** — Right-click a song and choose **Mark as Unplayed**.
- **Clear all** — Choose **Shows → Mark All Songs as Unplayed**.

Counts are for the current session only. They start fresh each time the profile opens, carry over when you switch shows, and come back after a crash restore.

## Crash Recovery

If Mx. Voice doesn't close normally, the next launch asks whether to restore the show in progress.

- **Restore show in progress** (or press **Return**) — Brings back the layout and played counts from when the app stopped.
- **Open saved show** — Opens the show as you last saved it. The show in progress is kept aside rather than deleted.

If only the window crashes, Mx. Voice offers to reload it and restores your show.

Closing the window now asks before quitting, so a stray click can't stop the music. **Quit** (**Exit** on Windows) in the menu still quits right away.

## Shows and Backups

[Profile backups](/docs/backups/) include your shows. Backups made before 4.4 have no shows: restoring one turns its layout into a show named Default Show. That layout may be from the middle of a performance rather than a prepared one. The restore confirmation tells you which shows a backup contains.

---
title: Moving to a New Machine
subtitle: Transfer your entire Mx. Voice setup with a single file
layout: ../../layouts/Docs.astro
---

## Overview

Starting in version 4.2.0, Mx. Voice includes a library import/export feature that lets you move your entire setup — songs, database, profiles, hotkeys, and settings — to a new machine using a single **.mxvlib** archive file. This also works across platforms (e.g., Mac to Windows).

## Exporting Your Library

1. Go to **File → Export Library...** in the menu bar.
2. Choose where to save the file. The default name is **MxVoice-Library.mxvlib**.
3. Click **Export**.
4. A progress bar shows the export status. When it's done, you'll see the total file size.
5. Click **Close**.

The export time depends on your library size. A large library with thousands of songs may take several minutes.

## What's Included in the Export

The .mxvlib file is a compressed archive containing everything you need to recreate your setup:

| Component | Details |
| --- | --- |
| **Song database** | All songs with their metadata (titles, artists, categories, info, durations). |
| **Audio files** | All music files in your audio directory. |
| **Profiles** | All user profiles with their individual preferences and state (holding tank contents, tab names, etc.). |
| **Hotkey files** | All saved .mrv hotkey configuration files. |
| **Settings** | Global preferences (fade duration, screen mode, etc.). Directory paths are automatically remapped on import. |

## Importing on the New Machine

1. Install Mx. Voice on the new machine.
2. Copy the **.mxvlib** file to the new machine (via USB drive, cloud storage, network share, etc.).
3. Launch Mx. Voice and go to **File → Import Library...**
4. Select the .mxvlib file.
5. A confirmation dialog appears showing details about the archive:
   - When and on what platform it was created
   - Number of music files, profiles, and hotkey files
   - Archive size
6. Click **Import and Replace** to proceed.
7. Wait for the import to complete. A progress bar shows each phase.
8. The application restarts automatically when finished.

After the restart, all your songs, profiles, hotkeys, and settings from the old machine are available.

> **Important:** Importing **replaces** all existing data on the new machine. There is no merge option. If you've already set up songs or profiles on the new machine, they will be overwritten.

## Cross-Platform Transfers

You can export on one platform and import on another (e.g., Mac to Windows, Windows to Linux). Mx. Voice handles the differences automatically:

- **File paths** are remapped to the new platform's default locations.
- **Filenames** are sanitized for compatibility (e.g., characters like `:` that are valid on Mac but not on Windows).
- **Window dimensions** from the source machine are not transferred — the new machine keeps its own window size.

## After Importing

The import sets all directory paths to default locations on the new machine. If you'd like to use custom directories, reconfigure them in [Preferences](/docs/preferences/) after importing.

## Tips

- The .mxvlib file uses ZIP compression, so a 10 GB music library might compress to 5–7 GB.
- You can cancel before clicking "Import and Replace" with no changes made. Once the import starts, it cannot be cancelled.
- Keep your .mxvlib file as a backup — it's a complete snapshot of your entire Mx. Voice setup.
- Both the source and destination machines should be running Mx. Voice 4.2.0 or later.

---
title: Troubleshooting
subtitle: Solutions to common issues and how to get help
layout: ../../layouts/Docs.astro
---

## Song Won't Play / File Not Found

If a song shows a warning icon and "File not found" in the playback bar, the audio file is missing from your audio files directory. This can happen if:

- The file was moved, renamed, or deleted outside of Mx. Voice.
- The audio files directory was changed in [Preferences](/docs/preferences/) without moving the files.
- The file was on an external drive that's no longer connected.

To fix this, either move the file back to the configured audio directory, or re-import it using the Add Song or Bulk Import features.

## Exporting Debug Logs

If you're experiencing an issue, debug logs can help diagnose the problem. Make sure debug logging is enabled in [Preferences](/docs/preferences/), then reproduce the issue.

To export your logs:

- **macOS:** Mx. Voice menu → **Export Logs**
- **Windows / Linux:** Help menu → **Export Logs**

This saves the last 7 days of logs to a single file that you can share with support. The exported file includes:

- App version, platform, and architecture
- Electron, Chrome, and Node.js versions
- All log entries with timestamps and severity levels

## Contacting Support

If you need help, there are several ways to reach us:

- **From the app:** Use the **Contact Support** menu item (in the Mx. Voice menu on macOS, or the Help menu on Windows/Linux). This opens your email client with a pre-addressed message to support@mxvoice.app.
- **GitHub Issues:** Report bugs or request features at [github.com/minter/mxvoice-electron/issues](https://github.com/minter/mxvoice-electron/issues).

> **Tip:** When reporting an issue, include your exported debug logs and a description of what you were doing when the problem occurred. This helps us diagnose the issue much faster.

## Audio Delay on Windows

On some Windows systems, the first song played after launching the app may have a 1–2 second delay. This is caused by the Web Audio context being suspended by the browser engine. Mx. Voice automatically resumes the audio context, and subsequent playback should be immediate.

## Missing Audio Files After Moving Directories

If you change your audio files directory in Preferences, your existing files are **not** moved automatically. You need to manually copy or move your audio files from the old directory to the new one. If you don't, songs in your library will show as "File not found" when you try to play them.

---
title: Managing Songs
subtitle: Add, organize, and manage your audio library
layout: ../../layouts/Docs.astro
---

## Supported Audio Formats

Mx. Voice supports the following audio formats:

- MP3 (.mp3)
- WAV (.wav)
- OGG (.ogg)
- FLAC (.flac)
- M4A (.m4a)
- MP4 (.mp4)
- AAC (.aac)

## Adding a Single Song

1. Open the **Add New Song** dialog.
2. Select an audio file from your computer.
3. Fill in the metadata:
   - **Title** (required) — auto-populated from the file's metadata if available, otherwise from the filename.
   - **Artist** — auto-populated from metadata.
   - **Category** (required) — select from existing categories or create a new one.
   - **Info** — optional notes or tags.
   - **Duration** — automatically calculated (read-only).
4. Click **Add** to save the song to your library.

The audio file is copied into your configured audio files directory with a unique filename to prevent conflicts.

## Bulk Import

The fastest way to build your library. Import an entire directory of audio files at once.

1. Open the **Bulk Add** dialog.
2. Choose a **source directory** containing your audio files.
3. Select a **category** for all imported songs (or create a new one).
4. Click **Add Songs**.

Mx. Voice scans the directory recursively (including subfolders) and for each audio file:

- Extracts metadata (title, artist, duration) from the file.
- Creates a database entry.
- Copies the file to your audio files directory.

## Editing Song Metadata

1. Select a song in the search results.
2. Open the edit dialog (double-click or use the edit action).
3. Update the **Title**, **Artist**, **Category**, or **Info** fields.
4. Click **Save**. The search results refresh automatically.

Duration cannot be edited — it's always calculated from the audio file.

## Deleting Songs

1. Select a song in the search results.
2. Press **Delete**.
3. Confirm the deletion in the dialog.

Deleting a song removes it from the database and deletes the audio file from your music directory. The song is also removed from any hotkey or holding tank assignments.

## Managing Categories

Categories help you organize your audio library. Each category has a short code (up to 4 uppercase letters) and a description.

### Creating a Category

1. Open the **Category Management** dialog.
2. Enter a description (e.g., "Sound Effects").
3. Click **Add**. A 4-letter code is auto-generated (e.g., "SOUN").

### Editing a Category

In the Category Management dialog, edit any category's description inline and click **Save Changes**.

### Deleting a Category

Click the delete button next to a category. All songs in that category are automatically reassigned to an "Uncategorized" category.

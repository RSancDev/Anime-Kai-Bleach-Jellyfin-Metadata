# Bleach Kai (Anime Kai) Jellyfin Metadata

I put this pack together to give **chjk122’s 35-part Bleach Kai edit** its own titles, summaries, and episode numbers in Jellyfin.

I’m not a coder. I’m just a dude who likes anime and wanted this to look right in my library. I had no idea how to make it, so I used AI to help create the metadata files, write the summaries, and organize everything. I figured I’d share it in case anyone else finds it useful.

<img width="1909" height="1052" alt="image" src="https://github.com/user-attachments/assets/d3d50462-487d-4ccf-992a-be6691830a93" />

## What’s included

- 35 episode NFO files with chapter titles, summaries, and numbering
- Series and season NFO files
- A master JSON file and episode mapping CSV
- The supplied source episode guide with usage percentages
- Checksums to verify the files

There are no videos, subtitles, or artwork in this repository.

## Download

[Download the metadata pack](https://github.com/RSancDev/Anime-Kai-Bleach-Jellyfin-Metadata/archive/refs/heads/main.zip)

## How to use it

1. Click **Code → Download ZIP** and extract it.
2. Open the `Bleach-Kai-chjk122-Metadata` folder and read `README.txt`.
3. Back up any NFO files you already have.
4. Copy each episode NFO into the same folder as its matching video. Their filenames need to match exactly, apart from the extension:

```text
Bleach 01 Soul Reaper.mkv
Bleach 01 Soul Reaper.nfo
```

Put `tvshow.nfo` in your series folder and `season.nfo` in the season folder if you use that layout. If your videos have different filenames, rename the NFO copies to match them.

Try one chapter first and check that Jellyfin picks up the correct title and summary before copying the rest.

## What’s been checked

All 37 NFO files passed XML checks, and the episode mappings match all 35 chapters in the supplied guide. The ZIP was also tested and extracted successfully.

An initial Jellyfin test picked up the first chapter’s title and summary, but it still appeared under **Season Unknown**. The full pack and season grouping have not been completely tested in Jellyfin.

### Example folder layout

Your Jellyfin media folder should look something like this:

```text
Bleach Kai/
├── tvshow.nfo
└── Season 01/
    ├── season.nfo
    ├── Bleach 01 Soul Reaper.mkv
    ├── Bleach 01 Soul Reaper.nfo
    ├── Bleach 02 Mod Soul.mkv
    ├── Bleach 02 Mod Soul.nfo
    └── ...remaining chapters
```

Each episode NFO goes beside its matching video and uses the exact same filename, apart from the extension. If your video filenames differ from these examples, rename the NFO files to match.

The videos shown above are your own files and are not included in this download.

## A few things to know

AI was involved in making this, so there may be mistakes. The summaries were written using the source episodes listed in the supplied guide. I haven’t checked every summary against the actual edited videos, so some details may describe scenes that were shortened or removed.

This pack only covers the 35-part Bleach Kai edit. It doesn’t cover TYBW, bonus content, or alternate versions.

If you spot a mistake or know a better way to set this up, feel free to open an issue or submit a correction. I’m learning as I go.

## Credits

All credit for the **Bleach Kai fan edit goes to chjk122**.

**Bleach was created by Tite Kubo.**

This is an unofficial community metadata pack. It isn’t affiliated with or endorsed by chjk122 or the original rights holders.

# 📺 IPTV Playlist

An automatically updated IPTV playlist repository powered by **GitHub Actions**.

This project collects and organizes IPTV/M3U sources into clean, categorized playlists that can be used with compatible IPTV players such as VLC, Kodi, TiviMate, and other M3U-compatible applications.

## ✨ Features

- 🔄 Automatic playlist updates
- ⚡ GitHub Actions automation
- 📺 M3U playlist format
- 🗂️ Organized channel categories
- 🧹 Playlist cleanup and formatting
- 🔗 Direct raw playlist URLs
- 📱 Compatible with M3U-supported IPTV players
- 🚫 Duplicate channel filtering
- ✅ Basic playlist validation

## 📁 Repository Structure

```text
.
├── .github/
│   └── workflows/
│       └── update-playlist.yml
│
├── sources.txt
├── playlist.m3u
└── README.md
```

## 🔗 Playlist

The generated playlist can be accessed through GitHub's raw file server:

```text
https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_REPOSITORY/main/playlist.m3u
```

Replace `YOUR_USERNAME` and `YOUR_REPOSITORY` with your GitHub username and repository name.

## 🔄 Automatic Updates

The playlist is automatically regenerated using GitHub Actions according to the schedule defined in:

```text
.github/workflows/update-playlist.yml
```

The workflow can:

1. Download configured M3U sources
2. Combine the playlist data
3. Validate the generated playlist
4. Detect changes
5. Commit updated content to the repository

## ▶️ How to Use

Copy the raw playlist URL and add it to any IPTV application that supports M3U playlists.

Example:

```text
https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_REPOSITORY/main/playlist.m3u
```

### VLC

Open:

**Media → Open Network Stream**

Then enter the playlist URL.

### IPTV Players

For applications supporting M3U URLs, add the raw playlist URL as an **M3U Playlist URL**.

## ⚙️ Configuration

Add your authorized M3U playlist sources to:

```text
sources.txt
```

Example:

```text
https://example.com/playlist1.m3u
https://example.com/playlist2.m3u
```

One URL should be placed on each line.

## ⚠️ Disclaimer

This repository is an automation and playlist-management project.

It does not claim ownership of third-party channels, logos, trademarks, or streaming content referenced by external sources.

Only use IPTV streams and playlist sources that you are authorized to access, aggregate, or redistribute. Users are responsible for complying with applicable copyright laws, licensing requirements, and the terms of the original stream providers.

## 📜 License

This project is provided for educational and playlist-management purposes.

If you add original code or other original content to this repository, you may choose an appropriate open-source license such as MIT.
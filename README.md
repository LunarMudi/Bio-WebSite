<div align="center">

<h1>
  <img alt="Mudi Avatar" src="assets/mudi.jpg" width="96" style="border-radius: 50%;">
  <br>
  Bio-WebSite
</h1>

**Bio-WebSite** is a professional, feature-rich, and fully customizable personal portfolio platform built with modern web technologies. It includes real-time Discord presence, Spotify integration, an immersive music player, advanced visual effects, customizable themes, and responsive design, delivering a premium user experience with zero external frameworks.

[Quick Start](#quick-start) ·
[Configuration](#configuration) ·
[Lanyard Setup](#lanyard-discord-status-setup) ·
[Features](#features) ·
[Repository Layout](#repository-layout) ·
[License](#license)

![Bio-WebSite Preview](https://bio.mudi.bio/assets/preview.png)

**Check out the live site at [bio.mudi.bio](https://bio.mudi.bio)**

This repository contains the complete HTML/CSS/JS source code for the Bio-WebSite.

</div>

---

## Quick Start

The website is fully static and requires no backend server. Simply open [`index.html`](index.html) in your browser, or serve the directory locally:

```sh
# Using Python
python -m http.server 8000

# Or using Node.js (http-server)
npx http-server

# Then open in browser
open http://localhost:8000
```

## Configuration

To fully customize your website, edit these files:
1. [`config.js`](config.js) - Main configuration (discord, theme, particles, bio, social links, music)
2. [`index.html`](index.html) - Meta tags, page title, and other HTML content
3. [`sitemap.xml`](sitemap.xml) - Your website's sitemap for SEO
4. [`robots.txt`](robots.txt) - Search engine crawler rules

Edit [`config.js`](config.js) to customize your website:

| Config Key | Description |
|------------|-------------|
| `discordUserId` | Your Discord user ID for live status integration (via Lanyard API) |
| `updateInterval` | Interval (ms) to refresh Discord status |
| `spotifyUpdateInterval` | Interval (ms) to refresh Spotify status |
| `defaultAvatarUrl` | Path to default avatar image |
| `siteAccentColor` | Default website accent color (hex code) |
| `particleColor` | Default particle effect color (hex code) |
| `maxParticleCount` | Maximum number of particles allowed |
| `displayName` | Your display name shown on the website |
| `espName` | Name shown in the ESP widget preview |
| `defaultTheme` | Default theme (light or dark) |
| `defaultMusicVolume` | Default music player volume (0-1) |
| `bioTexts` | Array of rotating bio texts for typing effect |
| `discordStatusTexts` | Custom status text for each Discord status (online/idle/dnd/offline) |
| `socialLinks` | Array of social links with icons, labels, and URLs |
| `musicPlaylist` | Array of songs for the built-in music player |

Example social link configuration:
```javascript
socialLinks: [
  {
    icon: "fas fa-server",  // Font Awesome icon class
    label: "databreach.vip", // Link label
    url: "https://databreach.vip" // Link URL
  }
]
```

Example music playlist entry:
```javascript
musicPlaylist: [
  {
    file: "songs/SongName/song.mp3", // Path to audio file
    title: "Song Title", // Song title
    artist: "Artist Name", // Song artist
    cover: "songs/SongName/cover.jpg" // Path to album cover
  }
]
```

## Lanyard Discord Status Setup

For the Discord status integration to work, you must join the official Lanyard Discord server:

👉 [discord.gg/lanyard](https://discord.gg/lanyard)

After joining, your Discord status will be available via the Lanyard API.

## Features

- 🟢 **Discord Status**: Live Discord status, activity, avatar, and Spotify integration via Lanyard API
- 🎵 **Music Player**: Built-in music player with playlist, shuffle, volume control, seek bar, and minimize option
- ✨ **Particle Effects**: Customizable particle system (count, speed, opacity, size) with interactive mode
- 🎨 **Theming**: Light/Dark theme support + custom accent and particle color pickers
- 🎯 **ESP Widget**: Stylish aimbot/ESP style widget for all customization controls
- 🖱️ **Custom Cursor**: Animated custom cursor effects
- 📱 **Responsive**: Works on mobile (music player hidden on mobile)
- 🔒 **Protection**: DevTools detection (redirects to GitHub), prevents copy/paste/context menu
- 📄 **404 Page**: Custom 404 error page that uses your saved theme/colors
- 🚀 **No Dependencies**: Standalone, no build tools required

## Repository Layout

| Path | Contents |
|------|----------|
| [`index.html`](index.html) | Main HTML structure and entry point |
| [`style.css`](style.css) | Complete styling with theme variables |
| [`config.js`](config.js) | User configuration (**not obfuscated**) |
| [`script.js`](script.js) | Application logic |
| [`assets/`](assets/) | Images, favicon, and banners |
| [`songs/`](songs/) | Music files and album covers |
| [`404.html`](404.html) | 404 error page |
| [`sitemap.xml`](sitemap.xml) | SEO sitemap |
| [`robots.txt`](robots.txt) | Search engine crawler rules |

## Star History

[![Star History Chart](https://api.star-history.com/chart?repos=LunarMudi/Bio-WebSite&type=date&legend=top-left&sealed_token=9ebxKvmV7pgsMjuHchYSqJcTe1E1rErges3V3ur2_Sf049zdkZ39D7QMxXhVI_t7r0wRAxeu79A40M00nCjB6X2UFbc9FDrg7sLv_YUZUDr5MzK0vV3FBdwnQIGXeIMNECPITHIiXoGUMLFILwzkJH5Ycs-7U2dhDSdgZ35QJN7zpgbdOMybJ2er9iUa)](https://www.star-history.com/?repos=LunarMudi%2FBio-WebSite&type=date&legend=top-left)

## License

Bio-WebSite is licensed under a custom license — see [`LICENSE`](LICENSE) for details.

Key license terms:
- ✅ You can use, copy, modify, and distribute the website for personal or non-commercial use
- ❌ You may NOT resell, rent, lease, or commercially exploit the website without permission
- 🔒 The footer (with copyright notice and GitHub link) **must remain intact and visible**
- 🔒 The DevTools/inspector protection (redirect to GitHub) **must NOT be removed or modified**

---

<div align="center">
  <p>
    <strong>© 2026 Mudi · All rights reserved</strong>
  </p>
  <p>
    <a href="https://github.com/LunarMudi/Bio-WebSite">
      <img src="https://img.shields.io/github/stars/LunarMudi/Bio-WebSite?style=social" alt="GitHub Stars">
    </a>
    <a href="https://github.com/LunarMudi/Bio-WebSite">
      <img src="https://img.shields.io/github/forks/LunarMudi/Bio-WebSite?style=social" alt="GitHub Forks">
    </a>
    <a href="https://github.com/LunarMudi/Bio-WebSite/blob/main/LICENSE">
      <img src="https://img.shields.io/badge/License-Custom-blue" alt="License">
    </a>
    <a href="https://mudi.bio">
      <img src="https://img.shields.io/badge/Website-mudi.bio-purple?logo=githubsponsors&logoColor=white" alt="Live Website">
    </a>
  </p>
</div>

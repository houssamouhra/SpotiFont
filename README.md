# SpotiFont

**Force the Spotify Mix font across the entire Spotify desktop app using Spicetify.**

> ⚠️ Works on desktop-only.

---

## Features

- Replace the old **Spotify Circular** font with the new **Spotify Mix** across all text in Spotify.  
- Works dynamically for newly loaded content.  
- Easy to use as a Spicetify snippet.  


---

## Compatibility

- **Older Spotify versions** (pre-1.2.27.xxxx / pre-May 2024): Fully enables the `Spotify Mix font` if missing. Ideal for users still on the old `Circular font`.  

- **Intermediate versions** (1.2.27.xxxx – 1.2.31.xxxx): Applies `Spotify Mix` across all UI elements for a consistent look, even if some fonts are partially updated.  

- **Latest Spotify versions** (post-May 2024 / 1.2.32+): Already include `Spotify Mix` by default.

- **Tested platform:** This project works with [Soggfy](https://github.com/Rafiuth/Soggfy), an alternative Spotify launcher.

---

## Installation

### 1. Install Spicetify

If you haven’t installed Spicetify yet, follow the [official Spicetify guide](https://spicetify.app/docs/getting-started/)

### 2. Add the Fonts

1. Open your Spicetify installation folder:
 - Windows: `C:\Users\<YourUsername>\AppData\Roaming\Spicetify`
 - macOS/Linux: `~/.config/spicetify/`

2. Inside the Spicetify folder, create a new folder called `Assets/Fonts`.
3. Copy the three `Spotify Mix` font files (`Regular`, `Bold`, `ExtraBold`) into this folder.

### 3. Add the Snippet

1. Open the **Spicetify Marketplace** --> **Snippets** --> **+Add CSS**.
2. Paste the following CSS snippet inside the **Custom CSS** input field:

```css

/* Album headers & metadata */
.main-entityHeader-container h1,
.main-entityHeader-pretitle,
.main-entityHeader-metaDataText,
.main-entityHeader-metaDataAuthor {
  font-family: "Spotify Mix", sans-serif !important;
  font-weight: inherit !important;
}

/* Track names, playlist titles, album titles */
.main-trackList-trackName,
.main-playlistTitle,
.main-albumTitle {
  font-family: "Spotify Mix", sans-serif !important;
  font-weight: inherit !important;
}

/* Sidebar, navigation, buttons, labels, context menus */
.main-rootlist-rootlistItemLink,
.main-navBar-navBarLink,
.main-contextMenu-menuItemButton,
.main-collectionLinkButton-collectionLinkText,
.queue-queue-title,
.queue-playHistory-title,
.connect-device-list a,
.main-buddyFeed-activityMetadata a,
.link-subtle,
input,
button {
  font-family: "Spotify Mix", sans-serif !important;
  font-weight: inherit !important;
}

/* Any other text in cards, modals, and UI elements */
.Text__TextElement-sc-if376j-0 {
  font-family: "Spotify Mix", sans-serif !important;
  font-weight: inherit !important;
}

```

### 4. Apply the Snippet

1. **Save your snippet** in Spicetify.
2. Run the following commands in your terminal (in the Spicetify folder)
```bash
spicetify apply
```

3. Restart Spotify to see the `Spotify Mix font` applied across the app.

---

## Notes

- This snippet works on the desktop version only and does not touch core Spotify files.

- Make sure your font files are properly named and placed in Assets/Fonts.

- This snippet overrides all text styling to Spotify Mix.

---

## License

Feel free to use, modify, and share. Attribution appreciated but not required.

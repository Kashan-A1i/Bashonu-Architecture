# 📸 Assets Checklist

Capture these from the **live app** and save them into `./assets/` with the **exact filenames** below. The README already links to them.

> [!IMPORTANT]
> **Before capturing:** use a test account, close DevTools (the Network tab shows the backend project URL), hide your browser bookmarks bar and extensions, and blur any real user emails or feedback comments. Use a clean browser profile at **1440×900** for desktop shots, or DevTools device mode at **390×844** (iPhone 14) for mobile shots.

---

### ☐ 1. `demo.gif`: hero walkthrough (about 15–25 s)
This is the most important asset. Record one continuous flow:
1. Land on **Home** in the *Light* theme and pause on the **Most Loved** / **New Additions** rows.
2. Type a **deliberately misspelled** query in the search bar (e.g. a poet name with a swapped vowel) to show fuzzy matches appearing live.
3. Tap a **language chip** to narrow the list.
4. Open a song, then tap the **theme toggle** (feather icon) to switch into **Paper** so the procedural parchment appears behind the lyrics.
5. Hit **fullscreen** (expand icon), zoom the font in with 🔍+, and exit.
6. Tap the **back button** to show Home restoring the exact scroll position.

**Tooling:** ScreenToGif (Windows) or Kap (macOS) at 12–15 fps, scaled to about 900 px wide, kept **under 8 MB** so GitHub renders it inline.

---

### ☐ 2. `song-paper-theme.png`: the procedural paper renderer
- Pick a song with **long lyrics** so the parchment fills the frame, in the **Paper** theme.
- Make sure the torn SVG-masked edges, the foxing spots and the vignette are all visible.
- *Bonus:* capture two different songs side by side to show that each song ID produces a unique, deterministic texture.

---

### ☐ 3. `script-toggle.gif`: Roman ⇄ Arabic script switch (about 4–6 s)
- Choose a song that has **both** Roman and Arabic-script lyrics.
- Toggle **Roman → Arabic → Roman** to show the RTL Nastaliq rendering and the change in line-height.
- *Alternative:* a still `script-toggle.png` with Arabic selected also works, but rename the README reference to match.

---

### ☐ 4. `admin-dashboard.png`: moderation and analytics
- Open `/admin` while logged in as an admin, on the **Feedback dashboard** view with the period set to **Last 30 days** or longer, so the average rating, star-distribution bars and comment feed are filled in.
- ⚠️ **Blur or crop any real feedback comments.** Better still, seed a few test entries first.
- *Optional second shot:* switch to **Song reports** and open a report in the modal, showing the Pending / Resolved / Dismissed status selector.

---

### ☐ Optional extras: `home.png` and `poet-page.png`
- **`home.png`**: Home on a **mobile viewport (390 px)** with the search bar, language chips and featured cards visible. This shows off the responsive layout.
- **`poet-page.png`**: a poet with a photo, birth/death years, a biography in Arabic script and at least one **memorable stanza** with a translation, scrolled so the hero and stanzas are both visible.

---

### Final check before pushing the showcase repo
- [ ] All files are in `./assets/` with the exact names above (`demo.gif`, `song-paper-theme.png`, `script-toggle.gif`, `admin-dashboard.png`, `home.png`, `poet-page.png`)
- [ ] No backend URLs, emails, auth tokens or real user comments are visible in any frame
- [ ] The live-site link and contact placeholders in `README.md` are filled in
- [ ] Each image is under about 2 MB (compress PNGs with TinyPNG or Squoosh), and GIFs are under 8 MB

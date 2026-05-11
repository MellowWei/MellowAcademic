# Wei Jueran — Academic Website
**魏珏然 · mellowwei.github.io**

Single-file academic site (`mellowwei-academic-full.html`) in a dark-cyber editorial format inspired by [dailynous.com](https://dailynous.com/). No build step, no dependencies beyond Google Fonts.

---

## File

```
mellowwei-academic-full.html   ← the entire site, one file
```

Deploy by dropping this file into any static host. For GitHub Pages, rename to `index.html` and push to your target repo/branch.

---

## Content included

| Section | Node |
|---|---|
| Scholar–Source Dual Channel | NODE 11 |
| BCI-HRP: The Human Return Protocol | NODE 01 |
| Vibration as Existence 振动即存在 | NODE 09 |
| Qualia Matrix | NODE 02 |
| PCR-QR Dual-Layer Diagnostic Framework | NODE 10 |
| Rhythm System 碎拍理论 | NODE 04 |
| Human Return Learning — MellowEd | NODE 12 |
| YourLanguage: Four Meta-Languages | NODE 13 |
| Gender Ontology 性别本体论 | NODE 14 |
| Love Sovereignty 爱的主权 | NODE 05 |
| Core Analytical Method (four-move) | — |
| Contact | — |

Non-academic nodes excluded: 星野愛, AiQ chat, Astro Time Candle, 闷声发大财, WhoYou.

---

## To update

**Add a new project entry** — copy any `<article class="entry">` block, change the `id`, badge class, title, description, and tags. Badge classes: `bp` (project/featured), `bpub` (publication), `br` (research), `be` (education), `bph` (philosophy).

**Update contact info** — search for `mellowwei7@gmail.com` and `laputamellow`; replace both instances in the contact article and the sidebar.

**Add Google Scholar / CV links** — find the two `href="#"` placeholders in the sidebar links block and the topbar.

**Change the 427Hz animation speed** — find `animation: pb 2.6s` in the CSS and adjust duration.

**Nav highlight** — driven by `IntersectionObserver` at the bottom of the file; add `id="yourId"` to any new `<article>` and a matching `<a href="#yourId">` in `.pnav` and it will auto-highlight on scroll.

---

## Deploy to GitHub Pages

```bash
# Option A — as a standalone page in MellowWei repo
cp mellowwei-academic-full.html index.html
git add index.html
git commit -m "academic site"
git push

# Option B — new repo, e.g. mellowwei.github.io/Academic
mkdir Academic && cp mellowwei-academic-full.html Academic/index.html
touch Academic/.nojekyll
# push Academic/ as a new repo or subfolder
```

---

## Fonts

Loaded from Google Fonts (requires internet):

- `Space Mono` — headers, labels, monospace UI
- `Spectral` — body text, italic titles, Chinese-adjacent serif
- `DM Sans` — general prose

To make the site fully offline, download these three families and host them locally, updating the `@import` at the top of `<style>`.

---

## Color tokens

| Token | Value | Use |
|---|---|---|
| `--a1` | `#5af0c8` | primary accent (427Hz teal) |
| `--a2` | `#9080f8` | secondary (purple, links, fields) |
| `--a3` | `#f07fd4` | research badge |
| `--a4` | `#f0c460` | education badge |
| `--bg` | `#07070f` | page background |
| `--hd` | `#edeaff` | headings |

---

*44271 · 427Hz · 振动即存在*

# Staging directory for the GitHub-side websites

Two GitHub repos get fed from here. Treat this folder as a staging area — write/edit here, then commit to the appropriate repo.

## `index.html` — for `mkadie/mkadie.github.io`

The personal page served at <https://mkadie.github.io/>. Two-part layout:

1. **Developer landing** (top, dark, terminal-style) — minimal orientation for anyone who arrives from a GitHub repo. Active repos, profile link, contact.
2. **Personal page** (R.O.A.R. design language) — about, background/credentials, current work, writing & research links, contact.

### To deploy

- Commit the file as `index.html` at the root of `mkadie/mkadie.github.io`.
- GitHub Pages auto-rebuilds in 30–60 seconds.

### Recent text changes vs. the prior draft

- *"Hi — I'm Michael."* → *"Hi — I'm Michael, I go by T-Rex."*
- Day-job line: *"Director of Engineering"* → *"Staff / Principal EV Engineer"* (stat lockup) and *"Staff / Principal Electric Vehicle Engineer (day job)"* (background card).
- *"I assumed he was smart…"* → *"I assumed he was **not** smart…"*  (this was a critical correction — the meaning was always that the assumption was wrong.)
- *"I'm in Chiang Mai…"* → *"I went to Chiang Mai…"*  (past tense; you're no longer there.)
- Writing & research card: the four Google Docs links are replaced with links to the new `.md` files in the NeedsBoard repo (see below). Each link shows the original date and the "updated to" date.

## `needsboard-docs/*.md` — for `mkadie/NeedsBoard`

Four design docs converted from Google Docs to Markdown. Each preserves the original as a snapshot and adds a "Status today" section reflecting where T-Rex Talk v3.0 stands now.

### To deploy

Commit the four files into the `mkadie/NeedsBoard` repo at `needsboard-docs/*.md`:

```
needsboard-docs/
├── project-overview.md
├── button-board-v1.md
├── needs-word-list.md
└── plan-going-forward.md
```

If you'd rather they live at the top level or under `docs/`, just adjust the paths — but if you change the location, update the matching links inside `index.html` so the personal page points to the right spot.

### What's in each file

| File | What | "Updated to" notes |
| --- | --- | --- |
| `project-overview.md` | The original "Moana associative device" design brief | T-Rex Talk v3.0 status, four supported hardware variants, devices deployed, related repos |
| `button-board-v1.md` | March 2025 PCA9555 / latch-circuit button board design | Replaced by `input_manager.py` and the four-variant model; original V1.0 design preserved |
| `needs-word-list.md` | Moana's six basic needs (the seed vocabulary). The original was a `.docx` that can't auto-export through the Google Docs API — this file holds the summary and pointers to the live `.menu` files | `.menu` files in the repo are now the canonical vocabulary store; original can be pasted in at the marker line |
| `plan-going-forward.md` | The pre-Open-Sauce-2025 plan, which the author noted "will not age well" | Status today: ✅ shipped, 🔄 in progress, future / queued |

### Commit message suggestion

```
Add design-doc snapshots from the original Google Docs

Each file preserves the early-2025 design brief and adds an "Updated"
section reflecting the T-Rex Talk v3.0 state. The originals stay in
Google Drive for reference; these are now the canonical Markdown
versions linked from the mkadie.github.io personal page.
```

## What this directory does NOT contain

- The `tssfaa.com` site lives at `C:\Users\live\OneDrive\assistive\website\`. Don't mix the two.
- The `ssi-racing.com` archive site lives at `Z:\websites\ssi-racing.com\`.
- The original Google Docs are still live — they haven't been deleted. The Markdown files supersede them as the canonical source going forward, but if a future caretaker wants the unedited originals, follow the doc links in the `index.html`'s footer-of-each-card meta line.

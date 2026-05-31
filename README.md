# mkadie.github.io

Personal page for **Michael Kadie** — I go by **T-Rex**. Served at <https://mkadie.github.io/>.

This repo is just one file, `index.html`, plus this README. No build step, no framework, no JavaScript bundler — GitHub Pages serves the HTML directly.

## What you'll find at the live site

Two parts, in order:

1. **Developer landing** — a small terminal-style block at the top for anyone who arrives from a GitHub repo. Quick links to the active repositories, the canonical project site, and contact.
2. **Personal page** — about me, my engineering background, the work I'm currently shipping, my writing and research, and how to reach me.

## The active work

Most of the day-to-day project information lives elsewhere — this page is just the entry point.

- **[tssfaa.com](https://tssfaa.com/)** — the public project site. R.O.A.R. (Rex's Open Assistive Resources), the schedule, MVP test-group recruitment, photo albums, press, and everything that ships.
- **[github.com/mkadie/NeedsBoard](https://github.com/mkadie/NeedsBoard)** — T-Rex Talk firmware, hardware files, build instructions. Tagged release [v3.0](https://github.com/mkadie/NeedsBoard/releases/tag/v3.0) shipped March 28, 2026.
- **[github.com/mkadie/SipNPuff](https://github.com/mkadie/SipNPuff)** — open-source breath-controlled switch. Working alpha/beta.
- **[github.com/mkadie/MSPM0_Seesaw](https://github.com/mkadie/MSPM0_Seesaw)** — Adafruit Seesaw-compatible I²C firmware for the TI MSPM0G3507.
- **[github.com/mkadie](https://github.com/mkadie)** — the rest of the public repositories.

## Editing the site

It's one `index.html`. Open it in any editor.

- Inline CSS at the top of the file uses the R.O.A.R. design tokens (same colours and fonts as `tssfaa.com`).
- All sections are anchored — the header nav uses `#about`, `#background`, `#writing`, `#contact`.
- Images load from `tssfaa.com` so there are no binary assets in this repo. If `tssfaa.com` is briefly unreachable, the page still renders fine; alt text shows in place of images.

After editing, commit and push. GitHub Pages auto-rebuilds in 30–60 seconds.

```
git add index.html
git commit -m "Update personal page"
git push
```

## Reach out

- Email — [main@tssfaa.com](mailto:main@tssfaa.com)
- GitHub — [@mkadie](https://github.com/mkadie)
- YouTube — [@but_Idigress](https://www.youtube.com/@but_Idigress)

*Heads up: I run an intentionally affordable mailbox, so replies sometimes land in spam. If you don't hear back in a couple of days, please check your spam folder.*

## License

The page content (the writing) is © Michael Kadie. The page styling builds on the R.O.A.R. design system used at `tssfaa.com` and is reused with attribution.

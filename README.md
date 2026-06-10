# Engineering the Strait

An interactive **scrollytelling** data story on backup-port selection for the
Merak–Bakauheni ferry crossing under peak (Eid) load — how an
optimization-and-simulation model cuts gridlock by ~68% for a 3.4× benefit-to-cost ratio.

Based on the final project (Tugas Akhir) of **Galih Mahastra Adhikararaksaka**,
Dept. of Marine Transportation Engineering, Institut Teknologi Sepuluh Nopember (ITS).

## Live

GitHub Pages: enabled on this repo (see the repo's Pages settings for the URL).

## Tech

- Single self-contained `index.html` — no build step.
- Dark "night chart" theme: deep navy, glowing teal water, amber accents.
- [D3.js](https://d3js.org/) for the sticky, scroll-synced visualizations.
- Scene-manager chart transitions: each step renders into its own SVG layer and
  crossfades with the previous one, so the panel never blanks between steps.
- [Lenis](https://github.com/darkroomengineering/lenis) for smooth, RAF-driven scrolling,
  plus a scroll-linked progress bar, hero parallax, and gentle panel float.
- `IntersectionObserver` (centre-of-viewport focus band) to sync narrative steps with charts.
- Chapter dot navigation (right rail, desktop) and count-up key numbers.
- Animated hero: drifting wave contours, coast silhouettes, a ferry commuting the strait.
- Respects `prefers-reduced-motion` (smooth scroll, parallax + heavy animation disabled).

## Develop

Just open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

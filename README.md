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
- [D3.js](https://d3js.org/) for the sticky, scroll-synced visualizations.
- [Lenis](https://github.com/darkroomengineering/lenis) for smooth, RAF-driven scrolling.
- `IntersectionObserver` (centre-of-viewport focus band) to sync narrative steps with charts.
- Respects `prefers-reduced-motion` (smooth scroll + heavy animation disabled).

## Develop

Just open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

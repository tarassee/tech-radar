# Tech Radar

Personal tech radar with per-year snapshots, live at **https://tarassee.github.io/tech-radar/**

Built on the [Zalando Tech Radar](https://github.com/zalando/tech-radar) visualization (MIT).

## Updating

Edit [`docs/config.json`](docs/config.json) and push to `master` — GitHub Actions redeploys the site automatically. Add a new year by adding a key under `years`; the toggle buttons are generated from those keys, and the latest year is selected by default.

Entry format:

```json
{ "label": "Kafka", "quadrant": 2, "ring": 0, "moved": 1 }
```

- `quadrant`: 0 = Languages & Frameworks, 1 = Platform & Infrastructure, 2 = Data Management, 3 = Techniques, Tools & AI
- `ring`: 0 = Adopt, 1 = Trial, 2 = Assess, 3 = Hold
- `moved`: 0 = no change, 1 = moved up, -1 = moved down, 2 = new

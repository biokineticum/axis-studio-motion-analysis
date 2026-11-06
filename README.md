# Axis Studio Motion Analysis

**Browser tool for Axis Studio Excel exports** — jump-height and gait analysis with Chart.js visualizations.

For coaches, physios and researchers using Perception Neuron / Axis Studio tabular exports.

Live: [biokineticum.github.io/axis-studio-motion-analysis](https://biokineticum.github.io/axis-studio-motion-analysis)

## Features

- Upload `.xlsx` Axis Studio–style exports in the browser (SheetJS)
- **Jump analysis** — vertical hip position (`Hips-Joint-Posi-y`), peak detection, height stats
- **Gait analysis** — hip / foot sensor accelerations, step-oriented metrics and charts
- Sample files in the repo: `jump_chr01.xlsx`, `walking_chr01.xlsx`
- Static GitHub Pages deploy (`.github/workflows/static.yml`)

## Quick start

Open the live site, or serve locally:

```bash
git clone https://github.com/biokineticum/axis-studio-motion-analysis.git
cd axis-studio-motion-analysis
python -m http.server 8080
```

Visit http://localhost:8080 — upload a sample workbook, pick Jump or Gait, run analysis.

## Data tips

- Jump demo uses hip vertical position with settings such as 60 Hz sampling in the app
- Gait demo expects hip and optional foot accelerometer columns following Axis Studio naming

## License note

Non-commercial / research use intended; for commercial licensing contact via [biokineticum.com](https://biokineticum.com).

---

## Author

**Dariusz Mosler** (Biokineticum) — physiotherapy, biomechanics, sports science  
🌐 [biokineticum.com](https://biokineticum.com) · 📰 [Substack](https://biokineticum.substack.com) · 𝕏 [@Biokineticum](https://x.com/Biokineticum)


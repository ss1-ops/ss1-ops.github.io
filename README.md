# ss1-ops.github.io

Professional single-page portfolio for Sam Snyder — Robotics Engineer & Automation Specialist (Precision Mechatronics, ROS2, PLCs, DFM/DFA, high-rate production).

**Live:** [https://ss1-ops.github.io](https://ss1-ops.github.io) • [https://samhsnyder.com](https://samhsnyder.com)

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-active-222222?logo=github)](https://ss1-ops.github.io)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-CDN-38B2AC?logo=tailwind-css)](https://tailwindcss.com)
[![Zero Build](https://img.shields.io/badge/Zero%20Build-true-000000)](https://github.com/ss1-ops/ss1-ops.github.io)

## Features

- **Single-file HTML** (`index.html`) with Tailwind CSS loaded via CDN — zero build step, zero dependencies, fully static.
- Clean, modern, dark-mode design with responsive layout.
- Sections: Header/hero, About (with key metrics), Experience (timeline with detailed achievements), Featured Projects (clickable cards that link directly to the corresponding GitHub repos), Skills (categorized tags), Education, Contact.
- Embedded downloadable CV (PDF).
- Project cards now link directly to the public repos for each featured project (see below).
- Custom domain via CNAME + GitHub Pages.

## Local preview

```bash
python -m http.server 8000
# or
npx serve .
```

Open http://localhost:8000 (or the port shown).

## Update process

1. Edit `index.html` directly (Tailwind classes via CDN, vanilla JS for interactivity like smooth scroll and theme toggle).
2. Commit and push to `main`.
3. GitHub Pages deploys automatically.

The site is hand-maintained as the single source of truth for the public-facing portfolio. No external CMS or generator.

## Featured Projects (direct repo links)

Clicking the cards on the live site opens the GitHub repositories:

- [6-DOF Robotic Arm + Aero Hand](https://github.com/ss1-ops/robotic-arm-5-digit-manipulator) — ROS2 Jazzy, MoveIt2, ESP32-S3 micro-ROS, vision-guided pick-and-place, custom Aero Hand gripper.
- [FANUC RMI Mock + Moveo Bridge](https://github.com/ss1-ops/fanuc-demo) — Reverse-engineered FANUC RMI server; drives real physical Moveo arm with unmodified `fanuc_ucl` client (interview artifact).
- [Pascal Tags — Full Automation Stack](https://github.com/ss1-ops/nordson-syringe-robotic-automation) — PLC + robot + web HMI for chipless RFID production (5 µm tolerance, production scaling).
- [OpenSesame Auto Door Handle](https://github.com/ss1-ops/auto-door-handle) — ESP32-S3 BLE + SwiftUI iPhone app + 3D-printed mechanism (daily driver mechatronics example).

(Valstad QC gantry and Canyon Magnet winding examples are documented in the site but not yet in separate public repos.)

## Tech stack

- HTML5 + Tailwind CSS (via CDN for zero-build)
- Vanilla JavaScript (theme toggle, smooth scrolling, mobile menu)
- GitHub Pages hosting + custom domain (samhsnyder.com)
- .nojekyll for clean asset serving
- PDF CV embedded

## License

MIT — see [LICENSE](LICENSE).

## Source

This repository *is* the portfolio. All content is in `index.html` (plus the CV PDF).

For deeper demos, videos, or private repos, contact via the site.

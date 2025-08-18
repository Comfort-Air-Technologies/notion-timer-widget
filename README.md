# Comfort Air Notion Timer Widget

An embeddable Pomodoro-style timer widget for Notion (or any iframe), perfect for deep work, breaks, and quick context switching.

[![Live Demo](https://img.shields.io/badge/demo-online-blue)](https://comfort-air-technologies.github.io/notion-timer-widget/)

---

## Features
- Work / Break durations with customizable lengths  
- Auto-switch and auto-restart options  
- Keyboard shortcuts:
  - **Space** → Start / Pause  
  - **R** → Reset  
- Compact mode for smaller embeds  
- Theme selection (e.g. Comfort, Light, Contrast, Neon)  
- Custom colors, ring styles, and UI glow options via URL  
- Transparent background toggle for Notion embeds  
- Shareable links with pre-set labels, times, and behaviors  
- Optional completion actions: toast messages or redirect to a URL  

---

## Quick Start

Use the live demo directly or embed it in Notion:  
https://comfort-air-technologies.github.io/notion-timer-widget/

---

## URL Parameters Cheatsheet

| Param        | Example                       | Description                                                |
|--------------|-------------------------------|------------------------------------------------------------|
| `label`      | `?label=Deep%20Work`          | Displayed session title                                    |
| `mins`       | `&mins=50`                    | Work duration in minutes (1–240)                           |
| `break`      | `&break=10`                   | Break duration in minutes (1–120)                          |
| `autostart`  | `&autostart=1`                | Automatically start timer on load                          |
| `compact`    | `&compact=1`                  | Compact layout suited for small embeds                     |
| `autoswitch` | `&autoswitch=1`               | Switch from work to break automatically                    |
| `autorestart`| `&autorestart=1`              | After break, automatically restart work                    |
| `muted`      | `&muted=1`                    | Start with sound muted                                     |
| `bg`         | `&bg=transparent`             | Transparent background for Notion                          |
| `theme`      | `&theme=Comfort`              | Choose from `Comfort`, `Light`, `Contrast`, `Neon`         |
| `ring`       | `&ring=thick`                 | Progress ring style (“thin”, “normal”, “thick”)            |
| `glow`       | `&glow=1`                     | Enable glowing effect on the ring                          |
| `accent`     | `&accent=%230ea5e9`           | Primary accent color (hex-encoded)                         |
| `accent2`    | `&accent2=%2334d399`          | Secondary accent color                                     |
| `labelbar`   | `&labelbar=0`                 | Hide the label bar (useful in minimal embeds)              |
| `webhook`    | `&webhook=https://...`        | POST `start`/`done`/`reset` events to a URL                |
| `next`       | `&next=https://...`           | Redirect browser or Notion page on timer completion        |
| `toast`      | `&toast=Great%20job!`         | Show a pop-up message upon completion                      |

---

## Example Links

**Deep Work (50 / 10, start auto, glow ring):**  
https://comfort-air-technologies.github.io/notion-timer-widget/timer.html?label=Deep%20Work&mins=50&break=10&autoswitch=1&autostart=1&ring=thick&glow=1&theme=Comfort&bg=transparent

**Quick Estimate Block (25 / 5, compact, locked UI):**  
https://comfort-air-technologies.github.io/notion-timer-widget/timer.html?label=Estimate&mins=25&break=5&compact=1&lock=1&theme=Comfort&bg=transparent

**Guided Focus (30 / 5, toast + redirect):**  
https://comfort-air-technologies.github.io/notion-timer-widget/timer.html?label=Focus%20Session&mins=30&break=5&autostart=1&next=https%3A%2F%2Fyour-notion-page.com&toast=Well%20done!

---

## Local Development

```bash
git clone https://github.com/Comfort-Air-Technologies/notion-timer-widget.git
cd notion-timer-widget
npm install
npm start
```

---

## License
MIT © Comfort Air Technologies

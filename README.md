# 💡 Light Panel Card

[![hacs_badge](https://img.shields.io/badge/HACS-Custom-orange.svg)](https://github.com/hacs/integration)
[![GitHub release](https://img.shields.io/github/release/DEIN-USERNAME/light-panel-card.svg)](https://github.com/DEIN-USERNAME/light-panel-card/releases)
[![GitHub stars](https://img.shields.io/github/stars/DEIN-USERNAME/light-panel-card.svg)](https://github.com/DEIN-USERNAME/light-panel-card/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A custom Home Assistant Lovelace card to display all your lights and smart plugs
in a clean panel with **live timers**, **custom icons**, **visual editor** and
**lock/unlock protection**.

![Preview](https://raw.githubusercontent.com/DEIN-USERNAME/light-panel-card/main/preview.png)

---

## ✨ Features

| Feature | |
|---|---|
| 💡 Lights & 🔌 Smart Plugs in one card | ✅ |
| ⏱️ Live timer – shows how long a light is ON | ✅ |
| 🎨 Visual editor – no YAML needed | ✅ |
| 🎨 Custom tile background color | ✅ |
| 🔒 Lock entities behind a toggle | ✅ |
| 🔌 Auto icon detection by domain | ✅ |
| ✏️ Custom icon per entity | ✅ |
| 📱 Drag & drop sorting | ✅ |
| 🌙 Follows your HA theme | ✅ |
| 📊 Sensor values displayed | ✅ |

---

## 📦 Installation

### Via HACS (recommended)

1. Open HACS → Frontend
2. Click **⋮ → Custom repositories**
3. Add URL: `https://github.com/DEIN-USERNAME/light-panel-card`
4. Category: **Lovelace**
5. Install **Light Panel Card**
6. Reload browser

### Manual

1. Download `dist/light-panel-card.js`
2. Copy to `/config/www/light-panel-card.js`
3. Add resource in HA:
   - **Settings → Dashboards → ⋮ → Resources**
   - URL: `/local/light-panel-card.js`
   - Type: `JavaScript Module`
4. Reload browser with `CTRL+SHIFT+R`

---

## ⚙️ Configuration

### Minimal

```yaml
type: custom:light-panel-card
title: Meine Lichter
entities:
  - entity: switch.wohnzimmer
  - entity: light.kueche

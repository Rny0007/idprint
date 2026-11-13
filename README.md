# CutSheet / IDPrint Studio 🪪

> **Zero-dependency, privacy-first in-browser ID card and passport photo layout utility with millimeter-accurate print scaling.**

[![Live Demo](https://img.shields.io/badge/demo-live%20app-success?style=for-the-badge&logo=googlechrome&logoColor=white)](https://rny0007.github.io/idprint/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)
[![Vanilla JS](https://img.shields.io/badge/Zero%20Dependencies-100%25%20Vanilla%20JS-orange?style=for-the-badge)](index.html)
[![100% Private](https://img.shields.io/badge/Security-100%25%20Client--Side-green?style=for-the-badge)](index.html)

---

## 🌟 Overview

**CutSheet (IDPrint Studio)** is a lightweight, high-precision web utility designed for printing identity documents, PVC cards, and passport photo sheets on standard home or photo studio printers.

Most document printing tools either require cloud uploads (compromising personal identity data) or suffer from browser auto-scaling distortions that distort card dimensions. CutSheet runs **entirely in your browser client** using HTML5 Canvas and CSS Paged Media (`@page`), ensuring that printed cards match physical wallet slots and standard laminates to the exact millimeter.

---

## ✨ Key Features

- 🔒 **100% Private & Client-Side**: All image cropping, manipulation, and rendering occur locally inside the browser. No identity cards or photos are ever uploaded to any server.
- 📐 **True Millimeter Precision**: Built-in CSS Paged Media rules (`@page`) and explicit physical dimensions (`mm`) eliminate browser print scaling errors.
- 💳 **Standard Card Presets**:
  - **ISO/IEC 7810 ID-1 (CR80)**: 85.60 mm × 53.98 mm (Standard National IDs, Driver's Licenses, PAN Cards, Corporate Badges).
  - **Dual-Side Alignment**: Front and back side alignment markers for duplex or manual flip printing.
  - **Custom Scaling**: Adjustable millimeters with lock-aspect ratio.
- 📸 **Passport Photo Grid Generator**:
  - **Standard Passport (35 mm × 45 mm)**: European, UK, Indian, and Australian consular standards.
  - **Square Visa (2 in × 2 in / 51 mm × 51 mm)**: US Visa, OCI, and Schengen specifications.
  - Generates multi-photo gang sheets on 4×6 photo paper or A4 sheets.
- ✂️ **Cutting & Fold Guides**: Toggleable corner crop marks and dashed centerfold lines for clean rotary trimmer cutting.
- ⚡ **Zero Dependencies**: Pure HTML5, modern CSS3, and vanilla JavaScript in a portable, self-contained architecture.

---

## 🚀 Quick Start / Local Usage

### Option 1: Live Web App
Open the deployed application in any modern browser:
👉 **[https://rny0007.github.io/idprint/](https://rny0007.github.io/idprint/)**

### Option 2: Run Locally (Offline Mode)
Because CutSheet has zero dependencies, you can run it completely offline:

```sh
# Clone the repository
git clone https://github.com/Rny0007/idprint.git

# Navigate into the folder
cd idprint

# Open directly in your browser
# On Windows:
start index.html

# On macOS:
open index.html

# On Linux:
xdg-open index.html
```

---

## 🖨️ Printing Best Practices

To achieve exact physical dimensions on your printer:

1. Press **Ctrl + P** (Windows) or **Cmd + P** (macOS) to open the print dialog.
2. Under **More Settings**:
   - **Destination**: Select your physical printer or "Save as PDF".
   - **Paper Size**: Match your loaded paper (e.g., `A4` or `4×6 in`).
   - **Scale**: Set strictly to **`100%`** or **`Actual Size`** (do *not* use "Fit to printable area" or "Fit to page").
   - **Margins**: Set to **`None`** or **`Default`** (page margins are controlled by CutSheet's internal stylesheet).
   - **Options**: Enable **`Background graphics`** for border and guide visibility.

---

## 📁 Repository Structure

```text
idprint/
├── index.html               # Main modern CutSheet application with interactive UI
├── id_card_print_tool.html  # Standalone single-page utility tool variant
├── CNAME                    # Custom domain mapping
├── LICENSE                  # MIT open-source license
└── README.md                # Project documentation and print guide
```

---

## 🛡️ Privacy Guarantee

Identity documents contain sensitive personally identifiable information (PII). CutSheet contains **zero analytics trackers, zero telemetry, zero cookies, and zero backend APIs**. You can inspect the source code in [`index.html`](index.html) or disconnect your internet completely before loading your documents.

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

Developed and maintained by **Rahul Buriya ([@rny0007](https://github.com/rny0007))**.
Contributions, feature suggestions, and bug reports are welcome via [GitHub Issues](https://github.com/Rny0007/idprint/issues).

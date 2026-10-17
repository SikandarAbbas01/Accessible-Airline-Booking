# Gate 11: Accessible Booking Lab

An interactive, single-file web app for learning and practicing **WCAG 2.1 AA** accessibility testing. It is themed around an airline booking flow, so every widget (tabs, dialog, menu, form, buttons) feels like something you would actually find on a flight booking site.

No frameworks, no build step, no dependencies. Just open `index.html` in a browser.

![Gate 11 screenshot](screenshot.png)

**Live demo:** https://your-username.github.io/your-repo-name/

---

## Features

### 1. Check-in desk: Keyboard and ARIA
- **Tabs** with full arrow-key, Home and End support
- **Accordion** with `aria-expanded` and `aria-controls`
- **Modal dialog** using the native `<dialog>` element, with focus returned to the trigger on close
- **Menu button** with arrow-key navigation, Escape to close, and click-outside to close
- **Form validation** with an error summary, linked error messages, `aria-invalid` and `aria-describedby`
- **Live keyboard event log** showing each key pressed and the focused element

### 2. Cabin lighting: Contrast and zoom
- **Contrast checker** with a live ratio and pass/fail for normal text (4.5:1) and large text (3:1)
- **Suggest a passing color** button
- **Text size control** from 85% to 200% (WCAG 1.4.4)
- **Color vision simulation**: protanopia, deuteranopia, tritanopia and achromatopsia
- **Text spacing toggle** (WCAG 1.4.12)
- **Reflow guidance** for 320px width (WCAG 1.4.10)

### 3. Maintenance hangar: Remediation workshop
- **Before and after** comparison of a broken and a fixed "Book flight" button
- **Issue tracker** to log accessibility issues with severity and status

### 4. Pre-flight audit
- **Manual audit checklist** with a progress bar
- **Report generator** that includes checklist results and logged issues
- **Copy to clipboard** and **Print** support

### Themes
- Daylight, Night flight (dark) and High contrast

---

## Getting Started

### Run locally
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```
Then open `index.html` in any modern browser.

### Deploy with GitHub Pages
1. Make sure the main file is named `index.html`.
2. Push the project to GitHub.
3. Go to **Settings > Pages**.
4. Under **Source**, choose the `main` branch and `/ (root)`, then save.
5. Your site will be live at `https://your-username.github.io/your-repo-name/`.

---

## How to Use the Lab

| Test | How |
|---|---|
| Keyboard only | Use `Tab`, `Shift+Tab`, `Enter`, `Space`, arrow keys and `Esc` |
| Screen reader | Try NVDA (Windows), VoiceOver (macOS/iOS) or TalkBack (Android) |
| Zoom | Use the in-page +/- buttons and browser zoom up to 200% |
| Reflow | Narrow your browser window to about 320px |
| Contrast | Pick colors in the checker or use the suggestion button |
| Automated | Run axe DevTools, Lighthouse or WAVE against the page |

> **Note:** Automated tools catch only part of the WCAG issues. Always test with real assistive technology.

---

## WCAG 2.1 Criteria Covered

| Criterion | Where it is demonstrated |
|---|---|
| 1.4.3 Contrast (Minimum) | Contrast checker, before/after button |
| 1.4.4 Resize Text | Text size control |
| 1.4.10 Reflow | 320px guidance and responsive layout |
| 1.4.12 Text Spacing | Text spacing toggle |
| 2.1.1 Keyboard | Tabs, menu, dialog, accordion |
| 2.4.1 Bypass Blocks | Skip link |
| 2.4.3 Focus Order | Logical tab order, dialog focus handling |
| 2.4.7 Focus Visible | Amber focus ring with dark outline |
| 3.3.1 / 3.3.3 Error Identification and Suggestion | Passenger form validation |
| 4.1.2 Name, Role, Value | ARIA roles and states on custom widgets |

---

## Project Structure

```
.
├── index.html      # The whole app: HTML, CSS and JavaScript
├── screenshot.png  # Preview image (optional)
└── README.md
```

## Built With
- HTML5 (semantic elements, native `<dialog>`)
- CSS3 (custom properties for theming, grid, flexbox)
- Vanilla JavaScript (no libraries)
- SVG filters for color vision simulation

## Browser Support
Latest versions of Chrome, Edge, Firefox and Safari.

## Contributing
Contributions are welcome.
1. Fork the repository
2. Create a branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push the branch: `git push origin feature/your-feature`
5. Open a pull request

## License
This project is licensed under the MIT License.

## Author
**Your Name**
GitHub: [@your-username](https://github.com/your-username)

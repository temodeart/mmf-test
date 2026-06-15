# Money Market Fund — Mobile App (Test build)

Interactive, browser-based prototype of the **Money Market Fund / Мони Маркет Фанд ХХК**
mobile app, generated from the design-system bundle (`DA→CL` export, contract v1.0).
It mimics the mobile app so the 99 screens can be clicked through and tested.

**Live site:** https://temodeart.github.io/mmf-test/

## How it works
- `index.html` — host harness: phone frame, hash router, navigation engine, screen menu.
- `screens.js` — all 99 screens precompiled from JSX (each registers to `window.__MMF_SCREENS`).
- `app.css` — shared animation / slider / scrollbar CSS used by the screens.
- `assets/` — official logo marks.

## Navigation
- **Tap inside the phone** — buttons, list rows, bottom-tab bar, and back arrows are wired
  to move between screens.
- **Every screen has its own URL** via hash routing, e.g.
  `…/mmf-test/#/Home`, `…/mmf-test/#/PrimaryBuyReview`.
- **Screens (☰)** — jump to any of the 99 screens, grouped by flow and searchable.
- **Back / Home / Next** — top-bar controls; Next follows the primary flow of the current screen.

Generated for testing purposes; not production code.

# Reindustrialize 2026 — Interactive Calendar

A single-file, interactive Google Calendar–style week view for the **Reindustrialize 2026** summit and side-events in Detroit (June 15–18, 2026).

No build step, no dependencies — just open `index.html` in any browser.

## Features

- **GCal-style week view** — Sun Jun 14 → Sat Jun 20, 2026, with an hour grid, all-day row, and a live "now" line (shown only when the real current date falls inside the viewed week).
- **Click-to-expand details** — clicking any event opens a slide-in panel with time, location, organizer, description, RSVP link, busy/visibility status, and reminder.
- **Overlap handling** — concurrent events split into side-by-side columns using the same column-packing + expansion algorithm Google Calendar uses (see the dense Tuesday morning: Cup of Capital + nTop booth + Summit).
- **Cross-midnight events** — late parties (e.g. 8:30 PM → 12:30 AM) clamp their block to midnight and show a `(+1 day)` marker in the detail panel.
- **Color-coded by category** — official summit (blue), parties (purple), tours (green), exhibitor/wellness (teal), socials (orange), dinner (lavender).
- **Week navigation** — prev / next / Today, with a panel that pushes the grid on wide screens and floats as an overlay on narrow ones.

## Events

All 20 events (official summit days + side-events) sourced from the Side Guide Detroit listing, with times, locations, hosts, access requirements, and RSVP links.

## Usage

```bash
open index.html
# or serve it:
python3 -m http.server 4601   # then visit http://localhost:4601
```

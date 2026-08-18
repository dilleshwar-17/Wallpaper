# Wallpaper

A dynamic desktop wallpaper built for **Lively Wallpaper** — featuring a liquid-glass design with a flip clock, daily motivational quotes (rotating every 2 minutes), and a fully featured to-do list widget.

## Features

- **Flip clock** — animated hour/minute/second display with multiple format options
- **Dynamic quotes** — 100 hand-picked motivational quotes across 10 categories, rotating every 2 minutes
- **To-do list widget** — add, edit, complete, and delete tasks directly on your wallpaper
  - Schedule due dates (Today / Tomorrow / +2 / +3 / +7 days)
  - Recurring tasks (Daily / Weekly / Monthly)
  - Day-wise overview (Previous / Today / Future)
  - Reminder banner for due/overdue tasks
  - Progress counter (`0/3 done`) on the widget
- **Liquid Glass UI** — frosted-glass panels, animated gradient blobs that shift color every 15 minutes
- **Customizable** — clock format, clock size, accent color, quote category, and widget toggles

## Installation Guide

### Prerequisites

- **Windows 10 or 11**
- **Lively Wallpaper** installed from the Microsoft Store or from https://rocksdanister.github.io/lively/

### Option 1 — Download & drop (easiest, recommended)

1. Download this repository as a **ZIP**: click the green **Code → Download ZIP** button.
2. Open **Lively Wallpaper**.
3. **Drag & drop** the downloaded `Wallpaper-main.zip` file directly onto the Lively window (do **not** extract it first).
4. The wallpaper appears in your library — double-click it to apply.

> `LivelyInfo.json` sits at the root of the project, so the ZIP imports without any extra steps.

### Option 2 — Single-file package

1. Download **`FlipClockWallpaper.zip`** from the repository.
2. **Drag & drop** it onto the Lively window (or double-click it).
3. Apply it from your library as usual.

### Option 3 — Install from source (git clone)

1. Clone the repository:

   ```sh
   git clone https://github.com/dilleshwar-17/Wallpaper.git
   ```

2. Open **Lively Wallpaper** → **Add Wallpaper** (`+`).
3. In the file picker, select the **`index.html`** file at the repo root (or drag the whole cloned folder onto the Lively window).

> ⚠️ Do **not** select `LivelyInfo.json` directly — Lively reports "file format not supported (.json)". That file is metadata only.

### Enabling the wallpaper

1. In Lively Wallpaper, your new wallpaper appears in the **Wallpaper library**.
2. Double-click it (or click **Apply**) to set it as your desktop wallpaper.

### Customization

Right-click the wallpaper (or open its settings in Lively) to adjust:

| Setting          | Description                              |
|------------------|------------------------------------------|
| Clock Format     | 12h/24h, with/without seconds/AM-PM      |
| Clock Size       | Slider from 0.5x to 2x                   |
| Accent Color     | Color of checkboxes and highlights       |
| Quote Category   | Discipline, Hard Work, Success, ...      |
| Show To-Do List  | Toggle the to-do widget on/off           |
| Show Quote       | Toggle the quote widget on/off           |

### Using the to-do list

- Type a task in the input box and press **Enter** (or click **Add**).
- Click the **checkbox** to complete a task.
- Click the **date/time chip** on a task to set a due date or make it recurring.
- Click **✎** to edit a task, **✕** to delete it.
- Click **☰ All** to open the full day-wise view (Previous / Today / Future).
- Overdue and due-today tasks show a reminder banner at the top of the screen.

## Project Structure

```
├── index.html            # Main wallpaper (layout, styling, logic)
├── LivelyInfo.json       # Lively Wallpaper metadata (at repo root, so the ZIP is directly importable)
├── LivelyProperties.json # Customizable settings exposed in Lively
├── quotes.js             # Bundled quote library (window.FCW_QUOTES)
├── FlipClock.umd.js      # Flip clock library
├── flipclock.css         # Flip clock styling
├── lively_t.jpg          # Library thumbnail
└── FlipClockWallpaper.zip# Pre-built single-file package for sharing
```

## License

This project is provided for personal use. Quote texts belong to their respective authors.
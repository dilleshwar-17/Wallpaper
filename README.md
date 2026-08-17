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
- Git (only if installing via `git clone`)

### Option 1 — Install from GitHub (recommended)

1. Open a terminal and clone the repository:

   ```sh
   git clone https://github.com/dilleshwar-17/Wallpaper.git
   ```

2. Open **Lively Wallpaper**.

3. Click **Add Wallpaper** (the `+` button) at the bottom-left of the Lively window.

4. In the file picker, navigate to the cloned folder, select the `LivelyWallpaper` folder, and choose `LivelyInfo.json` (or the whole folder).

5. Click **Open** — the wallpaper is now added to your library and will appear immediately on your desktop.

### Option 2 — Manual install (ZIP download)

1. Download the repository as a **ZIP** from GitHub (Code → Download ZIP).

2. Extract the ZIP to any folder, e.g. `C:\Users\<you>\Wallpaper`.

3. Open **Lively Wallpaper** → **Add Wallpaper** (`+`).

4. Select the `LivelyWallpaper` folder inside the extracted archive and choose `LivelyInfo.json`.

5. Click **Open** to add it to your library.

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
LivelyWallpaper/
├── index.html            # Main wallpaper (layout, styling, logic)
├── LivelyInfo.json       # Lively Wallpaper metadata
├── LivelyProperties.json # Customizable settings exposed in Lively
├── quotes.js             # Bundled quote library (window.FCW_QUOTES)
├── FlipClock.umd.js      # Flip clock library
└── flipclock.css         # Flip clock styling
```

## License

This project is provided for personal use. Quote texts belong to their respective authors.
# Intervals

Sub-41 10K training page (`index.html`).

`v2.html` is the same page plus a map of your route at the end of each run (pace-coloured line, km markers, GPX export). It shares saved runs and weights with `index.html`; `index.html` is unchanged.

The main link (`index.html`) now opens `v2.html`. To see the original page, open `index.html?v1`.

## Back up and restore (v2)

At the bottom of the v2 home page, under **Your data**:

- **Back up my data** saves everything the app keeps on the phone (every `sub41-…` item: runs, strength, padel, week changes, routes) into one file, `sub41-backup-YYYY-MM-DD.json`. On iPhone the share sheet opens so you can tap Save to Files; elsewhere the file downloads.
- **Restore from backup** reads a backup file, shows what's in it next to what's on the phone, and only replaces your data after you confirm.

## Treadmill runs (v2)

Every run type (easy, intervals, long, race) has an **Outdoor / Treadmill** choice on its start screen; Outdoor is the default.

- No GPS, route map or GPX on the treadmill. The screen stays awake as outdoors.
- Each pace becomes a treadmill speed in km/h, rounded to 0.1. A pace range uses the middle speed (easy 5:15–5:45/km = 10.4–11.4 km/h, aim 10.9). Recoveries between intervals are 8.0 km/h; strides are at interval speed.
- Coached by time: the speed to set is shown large and said at the start of each part, with a call 10 seconds before every change. Distance reps become a time at their speed (800 m at 15.2 km/h = 3:09).
- Km calls, the halfway call and encouragement use the estimated distance (speed × time), marked "~" on screen.
- At the end you're asked for the treadmill's distance (filled in with the estimate) and, optionally, its time.

Saved data: no names changed. Treadmill runs add new fields only (`env: "treadmill"`, `tm`, and `kmh` on reps and blocks). Runs without `env` are outdoor runs and are never re-written.

## Mark done (v2)

For a run or strength session you did without the app. **Mark done** sits next to **Start** on today's sessions, beside each session not yet done on today or an earlier day in **This week** (as padel already had), and under the Start button on the Run and Strength screens ("Done it without the app? Mark done").

- Runs: date, Outdoor / Treadmill, distance and time. The plan's distance and time are filled in to change; the average pace updates as you type.
- Strength: date and how long it took. No weights are logged, so weight suggestions still come from your last session in the app.
- The date starts as the day the session is planned for, or today if that's later. Future dates aren't allowed.
- It ticks off the session, counts towards the week, and shows in Activities and Recent runs marked "Manual". Open it to see its numbers, copy a summary or delete it.

Saved data: no names changed. Logged sessions are saved like ones done in the app, with one new field, `src: "manual"`; strength has no sets.

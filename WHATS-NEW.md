# Zelus update: new look and a smoother workout screen (Nov 25, 2026)

## New look
- The glowing gradient background, gradient headings and gradient buttons are gone. The app now uses solid dark-grey layers, one blue for anything you can tap or that shows progress, and gold only for personal records.
- Charts (weekly bars, progress lines, muscle split, 6-month calendar) match the new style and are easier to read. The line chart labels your latest value.
- Small buttons and filter chips are bigger (easier to hit with a thumb), and the grey hint numbers in set boxes are easier to read.

## Workout screen
- Each exercise shows "2 of 3 sets done" under its name, and turns green when finished.
- A progress bar under the timer tiles shows how far through the whole workout you are.
- The rest timer has a bar that drains as you rest, and tells you what is next (for example "Next up: Back Squat, set 3").
- A set that beats your record turns gold as soon as you tick it.

Your saved workouts, food and settings are untouched. Installed copies update on next open (offline cache zelus-v4).

# Zelus update: Hevy feature pass (Nov 24, 2026)

## Added to match Hevy
- Tracking types: weight & reps, bodyweight reps with optional added weight, assisted bodyweight, timed sets with a built-in stopwatch, distance & time. Custom exercises pick a type.
- Exercise page: rep records (best weight for 1+, 2+, 3+ ... reps), best set, best set volume, charts per type (1RM, heaviest, best set volume, session volume, total reps, longest hold, pace), how-to steps, last 10 sessions.
- New records: best set volume, most reps, longest hold, most added weight.
- Progress: weekly chart for volume, sets, reps, time or workouts; muscle split chart against the period before; sets per muscle per week with a 10-20 set band; 6-month training heatmap; monthly report with records and top exercises.
- Workout: replace an exercise, "muscles so far" map, workout notes, keep screen on, routine notes that carry into the workout, log a past workout, change date/time/length when editing.
- Share image of a finished workout.
- Settings: "last time" from any workout or same routine, rest timer sound, screen on, bar weight, plates you own.
- Body measurements: hips, shoulders, neck, forearm, calf added.

## Not copied (needs a native app or outside service)
Apple Watch / Wear OS, Apple Health, Strava sync, exercise leaderboards, video demos.

## Deploy
Same as before: Cloudflare Pages, no build command, KV binding named ZELUS.
The offline cache is now zelus-v2, so installed copies update on next open.

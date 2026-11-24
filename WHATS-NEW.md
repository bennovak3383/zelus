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

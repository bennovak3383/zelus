# Zelus review, Nov 25 2026

## Bugs found
1. **Rest timer never alerted while the workout was minimised.** The rest-end check lived inside the workout screen's timer element, so on Home/Food the beep and vibration did not fire, and then fired late when you reopened the workout. Fixed: the check now runs on every screen (`tick()`).
2. **Stale PR badge on a set.** The PR flag was computed only when a set was ticked. If you then corrected the weight or reps, or changed it to a warm-up, the badge stayed wrong and was saved into the finished workout. Fixed: the flag is recomputed on edit and on set-type change (`prFlag()`).
3. Service worker cache bumped to `zelus-v3` so installed phones pick up the new build.

## Friction vs Hevy (not yet changed)
- Exercise cards show no "2 of 3 sets done" progress, and the workout has no overall progress bar.
- The rest timer is a number only: no draining bar, no "next up" set. (Branch tracks the optional active-only field `restDur` in the workout draft to support a bar; old drafts without it load fine.)
- Small buttons and chips are 38px tall (under the 44px target). Placeholder text (#6f7888) is about 4:1 against the input background, and it carries the target weight/reps.
- The look leans on gradient washes: background glow with animated drift, gradient heading text, gradient buttons and hero card. This reads as "a little simple" and dated rather than premium.

## Data compatibility
No change to storage keys, the saved data shape, the sync API or auth. Workouts and food live in IndexedDB (`zelus` / `docs`); localStorage holds only `zelus:acc`, `zelus:lastSync`, `zelus:draft` and the `d:`/`dix` fallback.

## Next
1. Visual pass: layered dark-grey surfaces with one blue accent, an optional blue theme in Settings, 44px targets, refined tab bar, set rows, rest timer and chart styling, no gradient washes.
2. Workout flow: per-exercise set progress, an overall progress bar, a rest-timer bar with the next set named, and a gold highlight on the PR row.

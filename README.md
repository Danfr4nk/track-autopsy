# AUTOPSY — what did it?

A companion game to [MusicTrainer](https://github.com/Danfr4nk/MusicTrainer). MusicTrainer answers *whether* a track makes it. Autopsy answers **what it is about the track** that did it.

## The loop

Per track:
1. **Triage** — skip / like / ★ added (same ladder as MusicTrainer)
2. **Score** — 1–10 slider
3. **WHAT DID IT?** — check-all-that-apply across 16 production/musical/context drivers (drop, sound design, bass weight, vocal-as-texture, set utility…)
4. **KILL ONE** — remove one element and the track dies (identifies the load-bearing element)

## Drivers view

- **Lift ranking**: for each driver, how much more likely a track is to be a keep when you check it, vs your base keep rate. Min 2 checks; early leaders are suspects, not verdicts.
- **Load-bearing ranking**: frequency of KILL ONE picks — what your keeps are built on.

## Interop

Paste a **MusicTrainer week export** and every track arrives with its status + score intact — autopsy the drivers on top of real decisions. Or paste bare Spotify URLs.

## Method notes

- Check-all-that-apply (CATA) beats Likert scales for rapid profiling — tap what grabbed you, skip the rest.
- Vocals are texture, never words (lyric qualifier).
- Static site, no backend, no Spotify API. `localStorage` key `autopsy.v1`.
- Live at https://danfr4nk.github.io/track-autopsy/

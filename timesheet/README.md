# August 2026 — work hours

## What this is

A per-day timesheet for August 2026 with columns for **server**, **car**, and **other** hours,
plus the timestamp evidence I could recover for each day.

## What could not be reconstructed

**The server and car hours are blank, and I did not estimate them.** That work left no trace in
any system I can read:

- No repository named `server` exists. `lwiise/car.backend` exists but its last push was
  **2026-05-14** — nothing in August.
- No Claude Code session in August referenced either project (33 sessions checked, back to 2026-07-30).
- No local timesheet, log, or shell history — the working container is provisioned fresh.

Any per-day hour figure for server or car would have been invented. The columns are yours to fill.

## What the evidence does show

The `evidenced_window_utc` and `evidenced_span_h` columns are **hard timestamps from other
projects** — Fitlife, soul-and-body-landing, attica, mewseum-site, rindis-website,
signaturev1, inclusive-fit-website, virtual-scene-builder. They are useful as anchors: they show
which days you were demonstrably at a keyboard, and the shape of those working days.

Sources, all first-party:

| Source | What it proves |
|---|---|
| Claude session `created_at` | You started work at that moment |
| Claude session `updated_at` | You were still working at that moment |
| Published artifact `updated_at` | A document was written/revised at that moment |
| GitHub repo `pushed_at` | Code landed at that moment |

### Caveats

- **All times are UTC.** Your git commits carry `+0100`/`+0200`, so local time is 1–2h ahead.
  A 23:16 UTC timestamp on Aug 30 is past midnight local.
- **A span is a lower bound, not a duration.** `evidenced_span_h` is first-to-last evidence on
  that day. Real time at the keyboard may be less (you stepped away) or more (you worked before
  the first timestamp or after the last).
- **A single-point day has no span** — one timestamp proves the day, not the hours.
- **Blank is not proof of a day off.** It means nothing reached GitHub or Claude that day. This is
  exactly where the server and car work would be invisible.

## Summary of evidenced days (other projects)

- **14 of 31 days** carry activity: Aug 7, 11, 17, 19, 20, 21, 23, 24, 25, 26, 27, 28, 30, 31.
- **10 of those** have a bounded window, totalling **~30.2 h**.
- **17 days** have no recorded activity: Aug 1–6, 8–10, 12–16, 18, 22, 29.

The busiest stretch was **Aug 21 and Aug 23–28** — seven days out of eight, on the
soul-and-body-landing webinar and coach pages, then the Fitlife payments work.

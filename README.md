# taiwan-widget-data

Public data repo for the taiwan-widget Android app.

Contains `watchlist.json`, produced nightly at 20:30 TW by the
`taiwan-bullish-filter` Claude Code skill after its deep-analysis
pass. The Android app (private repo `taiwan-widget-android`) polls
the raw URL of this file and uses it as the source for its 觀察
(watchlist) screen, firing a notification when the live price drops
into an entry range.

Schema is documented in the `taiwan-bullish-filter` SKILL.md
step 3-6.

This repo is intentionally public so the app can fetch the JSON
without authentication. It contains only data, no code or secrets.

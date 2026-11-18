# earl-status

Where EARL (the EXAFS fitting web app at SLAC) is right now. `earl-link.json` is written by
`scripts/earl_status.sh` in the EARL repo whenever prod starts, restarts or stops, and is read by
https://stetef.github.io/earl/.

    {"status": "up" | "restarting" | "down", "url": "...", "since": "ISO 8601", "ends_at": "ISO 8601"}

Nothing secret lives here: the url is the public S3DF OnDemand link users click.

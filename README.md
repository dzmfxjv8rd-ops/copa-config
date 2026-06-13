# Copa version config

Remote version-gate config for the Copa iOS app, fetched on launch by `AppUpdateManager` (Linear INC-59).

- `minimum_version` — installs below this are **force-updated** (hard gate). Only bump to a version once it has cleared App Store review.
- `latest_version` — installs below this (but at/above `minimum_version`) get the **optional soft-update prompt**.
- `update_url` — App Store listing (`id6773815169`).

Edit `version.json` on each release. The app reads it fresh (no cache) on every launch; a failed fetch safely no-ops.

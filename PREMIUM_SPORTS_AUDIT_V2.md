# Premium Sports Audit V2

The previous audit produced false positives from `package-lock.json`. This corrected audit excludes lockfiles/dependency metadata and only accepts channel-like records or actual M3U entries.

- Real sports-like channel records discovered: **0**
- Probe budget used: **0**
- New names vs current V2: **0**

## Discovery notes
- High-Stability-IPTV-Service: discovered 0 playlist/database-like URLs; dynamic-endpoint hints in 0 files
- SHAJON-404 IPTV: discovered 2 playlist/database-like URLs; dynamic-endpoint hints in 6 files
- IPTVPulse-Daily-Updates: discovered 1 playlist/database-like URLs; dynamic-endpoint hints in 0 files
- SHAJON index not reachable at iamshajon.com/available_playlist.json: URLError
- SHAJON index not reachable at www.iamshajon.com/available_playlist.json: URLError

## Probe results

## Brand summary

| Brand/search term | Records | Reachable-like responses | Restricted 401/403 | Dead 404 | New names vs V2 |
|---|---:|---:|---:|---:|---:|

## Source summary

| Source | Records | Reachable-like responses | New names vs V2 |
|---|---:|---:|---:|

## Channel samples

Stream URLs are intentionally omitted.

| Channel | Source | Group | In V2? | Probe status |
|---|---|---|---|---|

## Important
- A media-like HTTP response does not prove a channel will play continuously or that it is authorized for redistribution.
- This audit does not use credentials, DRM keys, custom proxy bypasses, or access-control circumvention.
- The useful next step is to test any genuinely new, reachable channel names on your own player/device and compare stability against V2.
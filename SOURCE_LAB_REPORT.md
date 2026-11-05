# IPTV Candidate Source Lab

This repository tests the three candidate GitHub projects separately before anything is merged into the main V2 playlist.

| Source | Candidate files | Unique stream-like URLs | New vs V2 | Sample reachable % | Main probe outcomes |
|---|---:|---:|---:|---:|---|
| High-Stability-IPTV-Service | 0 | 0 | 0 | 0.0% |  |
| SHAJON-404 IPTV | 3 | 2 | 2 | 0.0% | NETWORK_ERROR:1, DEAD_404:1 |
| IPTVPulse-Daily-Updates | 1 | 1 | 1 | 100.0% | HTTP_200:1 |

## What this lab does
- Clones each candidate repository independently.
- Finds playlist/database-like files and stream-like URLs.
- Compares exact stream URLs against the existing V2 playlist.
- Performs a small, lightweight reachability/media probe.
- Keeps the repositories separate so a bad source cannot damage the existing V2 playlist.

## What this lab deliberately does not do
- It does not publish or merge extracted stream URLs.
- It does not use credentials or leaked accounts.
- It does not bypass DRM, subscription checks, regional controls, authentication, or other access controls.

Review the per-source reports in `/reports` before deciding whether any source belongs in the main playlist.

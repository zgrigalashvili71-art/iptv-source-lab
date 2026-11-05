# SHAJON-404 IPTV

## Inventory
- Candidate files: **3**
- Files containing #EXTINF entries: **0**
- Unique stream-like URLs discovered: **2**
- Exact URL overlap with current V2: **0**
- URLs not already present in V2: **2**

## Lightweight reachability sample
- URLs tested: **2**
- Immediately reachable/media-like: **0 (0.0%)**

### Probe results
- NETWORK_ERROR: 1
- DEAD_404: 1

### Most common source domains in tested sample
- `${domain}`: 1
- `example.com`: 1

## Candidate files

| File | EXTINF entries | URLs | Stream-like URLs |
|---|---:|---:|---:|
| `app/api/iptv/channels/helper.ts` | 0 | 1 | 1 |
| `app/api/iptv/playlists/available/route.ts` | 0 | 1 | 1 |
| `app/components/player/PlaylistManagerView.tsx` | 0 | 1 | 1 |

## Interpretation
- `HLS_OK`, `DASH_OK`, or `MEDIA_OK` means the endpoint responded like playable media during a small probe.
- `AUTH_OR_RESTRICTED_401/403` may require legitimate authorization, regional availability, headers, or another provider requirement.
- `DEAD_404`, `TIMEOUT`, `TLS_ERROR`, and `NETWORK_ERROR` reduce reliability.
- This test does not bypass DRM, authentication, subscription checks, geo-restrictions, CORS, or other access controls.
- A high count does not automatically mean a better source; stability and compatibility matter more than raw channel count.

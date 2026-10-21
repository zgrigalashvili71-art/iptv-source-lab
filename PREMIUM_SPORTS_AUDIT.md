# Premium Sports Audit

This report checks whether the candidate sources contain premium-sports-branded channel names and whether a sample endpoint responds without using credentials, custom headers, proxies, DRM keys, or bypass techniques.

- Matching records discovered: **2**
- Endpoints probed: **2**
- Names also present in current V2: **0**
- Names not present in current V2: **2**

## Probe status summary
- **MEDIA_RESPONSE**: 2

## Brand summary

| Brand | Records | Reachable-response sample | Restricted 401/403 | Dead 404 | New names vs V2 |
|---|---:|---:|---:|---:|---:|
| ufc | 2 | 2 | 0 | 0 | 2 |

## Source summary

| Source | Matching records | Reachable-response sample | New names vs V2 |
|---|---:|---:|---:|
| `SHAJON-404 IPTV:package-lock.json` | 2 | 2 | 2 |

## Channel-name samples

The report intentionally does **not** publish stream URLs.

| Channel name | Brand | Source | Group/category | In current V2? | Probe status | Special metadata seen |
|---|---|---|---|---|---|---|
| 1.2.0 / sha512-5l4VyZR86LZ/lDxZTR6jqL8AFE2S0IFLMP26AbjsLVADxHdhB/c0GUsH+y39UfCi3dzz8OlQuPmnaJOMoDHQBA== / MIT | ufc | `SHAJON-404 IPTV:package-lock.json` |  | No | MEDIA_RESPONSE | drm_metadata |
| 2.2.1 / sha512-F+i2BKsFrH66iaUFc0woD8sLy8getkwTwtOBjvs56Cx4CgJDeKQeqfz8wAYiSb8JOprWhHH5p77PbmYCvvUuXQ== / MIT | ufc | `SHAJON-404 IPTV:package-lock.json` |  | No | MEDIA_RESPONSE | drm_metadata |

## How to interpret this
- `HLS_RESPONSE`, `DASH_RESPONSE`, or `MEDIA_RESPONSE` means the endpoint responded like media during a small probe.
- That does **not** prove the stream is authorized for redistribution or that it will remain stable.
- `RESTRICTED_401/403` means the endpoint refused the unauthenticated probe.
- `custom_headers`, `referer_or_origin`, `proxy_field`, or `drm_metadata` indicate the source record contains special playback metadata. This audit does not use those fields to circumvent access controls.
- `DEAD_404`, `TIMEOUT`, `TLS_ERROR`, and `NETWORK_ERROR` are poor signs for direct playback.

# AAPL Options Expiration Tracker

Weekly tracking repository for Apple (AAPL) options expirations, chain statistics, and risk-meeting prep. All market figures below are from live data pulled from Yahoo Finance at the time of this week's review.

## Company Snapshot (Apple Inc.)

| Field | Value |
| --- | --- |
| Headquarters street address | One Apple Park Way, MS 927-4GC |
| City | Cupertino (CA 95014, United States) |
| Sector | Technology |
| Industry | Consumer Electronics |
| Current share price | $355.63 (Yahoo Finance, NASDAQGS, USD) |
| Company | Apple Inc. (AAPL) |
| Analyst recommendation | Buy (mean 2.22, 40 analyst opinions) |
| Market cap | ~$5.168T |
| 52-week range | $243.42 – $355.90 |
| Previous close | $348.51 |
| Day range | $349.325 – $355.90 |
| Trailing P/E | 39.60 |
| Forward P/E | 33.70 |
| Beta | 1.089 |
| Date pulled | 2026-11-09 (per exchange data timestamps in source) |

## Expiration Map — Available AAPL Option Expirations

Full list returned by Yahoo Finance for AAPL (in order):

| # | Expiration Date |
| --- | --- |
| 1 | 2026-11-11 |
| 2 | 2026-11-13 |
| 3 | 2026-11-16 |
| 4 | 2026-11-18 |
| 5 | 2026-11-20 |
| 6 | 2026-11-27 |
| 7 | 2026-12-04 |
| 8 | 2026-12-11 |
| 9 | 2026-12-18 |
| 10 | 2026-12-24 |
| 11 | 2027-01-15 |
| 12 | 2027-02-19 |
| 13 | 2027-03-19 |
| 14 | 2027-04-16 |
| 15 | 2027-06-17 |
| 16 | 2027-09-17 |
| 17 | 2027-12-17 |
| 18 | 2028-01-21 |
| 19 | 2028-03-17 |
| 20 | 2028-06-16 |
| 21 | 2028-12-15 |
| 22 | 2029-01-19 |

**This week's focus (three soonest upcoming expirations, skipping anything earlier than today):**
1. **2026-11-11**
2. **2026-11-13**
3. **2026-11-16**

## Per-Expiration Chain Stats

**Share price used for ATM selection across all expirations: $355.63**

### Expiry 2026-11-11

| Metric | Value |
| --- | --- |
| ATM strike (closest to $355.63) | **$355** |
| Highest-OI Call strike | **$355** (`AAPL261111C00355000`, OI 33,155, volume 183,356) |
| Highest-OI Put strike | **$340** (`AAPL261111P00340000`, OI 5,854, volume 6,326) |

### Expiry 2026-11-13

| Metric | Value |
| --- | --- |
| ATM strike (closest to $355.63) | **$355** |
| Highest-OI Call strike | **$355** (`AAPL261113C00355000`, OI 11,813, volume 24,754) |
| Highest-OI Put strike | **$265** (`AAPL261113P00265000`, OI 10,654, volume 10,606) |

### Expiry 2026-11-16

| Metric | Value |
| --- | --- |
| ATM strike (closest to $355.63) | **$355** |
| Highest-OI Call strike | **$355** (`AAPL261116C00355000`, OI 5,737, volume 2,541) |
| Highest-OI Put strike | **$330** (`AAPL261116P00330000`, OI 1,537, volume 490) |

## Notes on Data Quality

- strike spacing on all three expirations includes $2.50 increments near the money ($332.50, $335, $337.50, $340, $342.50, $345, $347.50, $350, $352.50, $355, $357.50).
-Values above are reported exactly as returned by the Yahoo Finance option chain source; nothing has been normalized beyond selecting the strike closest to the current share price of $355.63.
- Open interest figures are as-of the latest available chain snapshot from the source.

## Repository Contents

- `expirations.md` — this file (company snapshot, full expiration map, per-expiration stats table)
- `CONTRIBUTING.md` — contributed on `main` via PR #4 (see PR description)
- Tracking issues #1 (2026-11-11), #2 (2026-11-13), #3 (2026-11-16)
- `.github/workflows/` — minimal manual-dispatch workflow for repo hygiene

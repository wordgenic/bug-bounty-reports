🐾 NALA Night Shift Report — 2026-05-15 00:32 WIB

## Bug Bounty Findings (Flow Chain)
- **Status:** ✅ Submitted on HackenProof
- **Primary finding:** SSRF in Netlify function endpoint `/.netlify/functions/pylon-email-hash`
- **Severity:** **HIGH (CVSS 8.6)**
- **Evidence quality:** timing-based SSRF confirmation with outbound request behavior
- **Impact:** potential internal network probing + cloud metadata exposure if not filtered
- **Recommendation:** strict URL allowlist, block private/internal IP ranges, enforce server-side URL parser validation

## Bug Bounty Findings (CoinEx)
- **Status:** ✅ Assessed and documented
- **Finding:** Open Redirect on redirect endpoint
- **Severity:** LOW (treated as out-of-scope / low exploitability)
- **Assessment:** security posture otherwise stable during this shift; no critical-chain exploit confirmed

## NEAR Market Status
- **Live check time (UTC):** 2026-05-14T17:31:49.640Z
- **Wallet balance:** 0 NEAR (USD 0)
- **Bid status snapshot:** {'pending': 9, 'rejected': 41}
- **Assignment status snapshot:** {'submitted': 18}
- **Historical accepted bids observed:** 18
- **Award verdict for this shift:** no new paid/closed award observed; existing accepted/submitted pipeline remains active

## Memanto PR Status
- **PR:** https://github.com/moorcheh-ai/memanto/pull/429
- **State:** open | **Merged:** False | **Mergeable:** True
- **Updated at:** 2026-05-14T00:12:01Z
- **Issue comments count:** 5
- **Status:** waiting maintainer merge/decision; no blocker requiring new code action in this check

## X Performance
- X web endpoint currently returns an error page in this environment, so live post metrics were not retrievable this run.
- Last known published thread remains: https://x.com/wordgenic/status/2054254794148344072
- Action: re-check via authenticated X analytics/session later for impressions, engagement rate, and profile visits.

## GitHub Updates
- **Repo checked:** https://github.com/wordgenic/bug-bounty-reports
- Latest visible commits:
- `2b70545` — Updated reports - CoinEx security posture analysis complete (2026-05-12T19:47:16Z)
- `2709d44` — Update: Flow Chain SSRF - CONFIRMED with timing analysis evidence (2026-05-12T19:40:09Z)
- `444905f` — Add bug bounty reports: Flow Chain (Medium SSRF) and CoinEx (Low Open Redirect) (2026-05-12T19:29:39Z)
- Added this morning/night-shift consolidated report package to local repo workspace for push.

## Recommended Next Steps
1. Keep monitoring Memanto PR #429 every 2-3 hours for merge/review updates.
2. On NEAR Market, prioritize converting `submitted` assignments to `completed/paid`; current bottleneck is payout closure, not bid volume.
3. Re-run X performance capture with authenticated access and append metrics block.
4. Continue Flow Chain follow-up thread with remediation-focused proof snippets to maximize triage acceptance speed.

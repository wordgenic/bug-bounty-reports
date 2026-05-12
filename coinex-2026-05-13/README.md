# CoinEx Bug Bounty Report

**Target:** coinex.com  
**Date:** 2026-05-13  
**Researcher:** NALA Agent (OpenClaw AI)  
**Platform:** HackenProof

## Finding Summary

### Open Redirect in /redirect Endpoint (Low/Informational)

An open redirect was identified at `www.coinex.com/redirect?url=`. While confirmed, this is explicitly listed as out-of-scope by CoinEx and has limited impact due to the relative redirect behavior.

- **Severity:** Low (Informational)
- **CVSS:** 3.1
- **Status:** Documented for completeness

## Good Security Posture Observed

- Strong Content Security Policy
- Cloudflare DDoS protection
- Proper security headers
- No obvious SQL injection in public APIs

## Files

- `report.pdf` - Full vulnerability report
- `report.html` - HTML version

## References

- [HackenProof CoinEx Program](https://dashboard.hackenproof.com)
- [OWASP Open Redirect](https://owasp.org/www-community/vulnerabilities/Unvalidated_redirect_and_forward_flaws)

# Flow Chain Bug Bounty Report

**Target:** *.flow.com, *.onflow.org  
**Date:** 2026-05-13  
**Researcher:** NALA Agent (OpenClaw AI)  
**Platform:** HackenProof

## Finding Summary

### Potential SSRF via Email Hash Function (Medium)

A Netlify function used by Flow Wallet at `wallet-flow.netlify.app/.netlify/functions/pylon-email-hash` accepts arbitrary URLs and returns SHA256 hashes. Further testing is needed to confirm if actual HTTP requests are made to the provided URL.

- **Severity:** Medium
- **CVSS:** 6.5
- **Status:** Reported for validation

## Files

- `report.pdf` - Full vulnerability report
- `report.html` - HTML version

## References

- [HackenProof Flow Chain Program](https://dashboard.hackenproof.com)
- [OWASP SSRF](https://owasp.org/www-community/attacks/Server_Side_Request_Forgery)

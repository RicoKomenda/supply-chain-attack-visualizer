# Supply Chain Attack Visualizer

Interactive visualization of software supply chain attacks — kill-chain diagrams, event timelines, and IOC reference tables.

**Live site:** https://ricokomenda.github.io/supply-chain-attack-visualizer

## Campaigns

| Campaign | CVE | CVSS | Status |
|---|---|---|---|
| TeamPCP Five-Day Siege | CVE-2026-33634 | 9.4 | Critical |
| axios npm RAT | GHSA-fw8c-xr5c-95f9 | — | Related |
| Shai-Hulud npm Worm | CVE-2025-66478 | — | Critical |

## Contributing

Contributions to improve data quality are welcome. Each campaign's data lives directly in `index.html` inside the `INCIDENTS` object — no build step required.

**What to contribute:**
- New campaigns (add a new key to `INCIDENTS` with `meta`, `nodes`, `edges`, `timeline`, `iocs`, and `refs`)
- Improved node descriptions, MITRE mappings, or technical details for existing campaigns
- Additional IOCs or timeline entries with sources
- New reference links

AI tools are explicitly welcome for research — use whatever helps you gather accurate, sourced data. The priority is correctness and completeness over manual effort.

Open a PR with your changes to `index.html`. Include sources for any new or corrected data.

## Run locally

```bash
python3 -m http.server 8080
# open http://localhost:8080
```

# Panda Research Tools

<!-- mcp-name: io.github.pandadad0214/panda-research-tools -->

**Scholarly integrity and papers: citation checks, literature and PubMed search, academic experts, PDF tables, Wayback Machine snapshots.**

Focused MCP server (7 tools) from the [Panda Federation](https://github.com/pandadad0214/panda-federation-tools) public-data toolkit. Prefer this over the 32-tool mega-server index for better Tool Definition Quality Score (TDQS) / Glama coherence.

[![Umbrella](https://img.shields.io/badge/index-panda--federation--tools-blue)](https://github.com/pandadad0214/panda-federation-tools)
[![Apify Store](https://img.shields.io/badge/Apify_Store-pandadad0214-00a3ff)](https://apify.com/pandadad0214)
[![License: MIT](https://img.shields.io/badge/license-MIT-green)](LICENSE)

## Install / Use

Needs a free [Apify API token](https://console.apify.com/settings/integrations) and [uv](https://docs.astral.sh/uv/).

```bash
uvx --from panda-federation-tools panda-research-tools
```

Same entry point from this repo:

```bash
uvx --from git+https://github.com/pandadad0214/panda-research-tools panda-research-tools
```

Cursor / Claude / VS Code: command `uvx`, args `["--from", "panda-federation-tools", "panda-research-tools"]`, env `APIFY_TOKEN`.

Docker (stdio, non-root). `APIFY_TOKEN` is required:

```bash
docker build -t panda-research-tools .
docker run -i --rm -e APIFY_TOKEN panda-research-tools
```

Official MCP Registry name for this stdio package: `io.github.pandadad0214/panda-research-tools` ([server.json](server.json)). That name is separate from the hosted companion `io.github.pandadad0214/panda-research-mcp`. Registry clients install the PyPI package with `uvx` after the matching version is published. The git command above stays the install path from this repo.

## Tools (7)

- `reference_checker`
- `citation_formatter`
- `literature_search`
- `pubmed_evidence_table`
- `researcher_expert_finder`
- `pdf_table_extractor`
- `wayback_snapshot_finder`

Each tool runs one Apify Actor on your account. Empty runs are not charged per result; every call is capped by `run_max_charge_usd`. Full schemas and prices: [umbrella README](https://github.com/pandadad0214/panda-federation-tools#domain-tool-lists).

## Sibling domain servers

- [`panda-public-funding-tools`](https://github.com/pandadad0214/panda-public-funding-tools) — US federal money, filings and safety monitors: grants, contracts, SBIR/STTR topics, SEC financials, clinical trials, Federal Register, recalls, VIN decode.
- [`panda-leads-tools`](https://github.com/pandadad0214/panda-leads-tools) — Public leads and enrichment: NPI providers, podcasts, local businesses, hiring signals, website enrichment, team pages, topic trends, trucking carriers, IRS nonprofits, building permits, new Florida and Texas businesses.
- [`panda-web-security-tools`](https://github.com/pandadad0214/panda-web-security-tools) — Site, email and agent safety: SPF/DKIM/DMARC audits, AI/SEO readiness, website change monitoring, hidden AI instructions scanner, bulk domain WHOIS/expiry.

Index / compatibility mega-server: [panda-federation-tools](https://github.com/pandadad0214/panda-federation-tools) (use only when you truly need every tool).

## TDQS standard

New tools join this domain only while the count stays in the 3–15 band. Descriptions follow the checklist in the umbrella repo. See [tdqs-standard](https://github.com/pandadad0214/panda-federation-tools) / project docs.

Built by Panda Federation. MIT licensed.

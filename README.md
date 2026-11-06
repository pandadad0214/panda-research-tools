# Panda Research Tools

**Scholarly integrity and papers: citation checks, literature and PubMed search, academic experts, PDF tables.**

Focused MCP server (6 tools) from the [Panda Federation](https://github.com/pandadad0214/panda-federation-tools) public-data toolkit. Prefer this over the 23-tool mega-server for better Tool Definition Quality Score (TDQS) / Glama coherence.

[![Umbrella](https://img.shields.io/badge/index-panda--federation--tools-blue)](https://github.com/pandadad0214/panda-federation-tools)
[![Apify Store](https://img.shields.io/badge/Apify_Store-pandadad0214-00a3ff)](https://apify.com/pandadad0214)
[![License: MIT](https://img.shields.io/badge/license-MIT-green)](LICENSE)

## Install / Use

Needs a free [Apify API token](https://console.apify.com/settings/integrations) and [uv](https://docs.astral.sh/uv/).

```bash
uvx --from git+https://github.com/pandadad0214/panda-research-tools panda-research-tools
```

Or, once `panda-federation-tools` ≥ 1.4.0 is on PyPI:

```bash
uvx --from panda-federation-tools panda-research-tools
# same entry point, no thin-repo clone required
```

Cursor / Claude / VS Code: command `uvx`, args `["--from", "git+https://github.com/pandadad0214/panda-research-tools", "panda-research-tools"]` (or `["--from", "panda-federation-tools", "panda-research-tools"]`), env `APIFY_TOKEN`.

## Tools (6)

- `reference_checker`
- `citation_formatter`
- `literature_search`
- `pubmed_evidence_table`
- `researcher_expert_finder`
- `pdf_table_extractor`

Each tool runs one Apify Actor on your account. Empty runs are not charged per result; every call is capped by `run_max_charge_usd`. Full schemas and prices: [umbrella README](https://github.com/pandadad0214/panda-federation-tools#domain-tool-lists).

## Sibling domain servers

- [`panda-public-funding-tools`](https://github.com/pandadad0214/panda-public-funding-tools) — US federal money and filings: grants, contracts, SBIR/STTR topics, SEC financials, clinical trials.
- [`panda-leads-tools`](https://github.com/pandadad0214/panda-leads-tools) — Public leads and enrichment: NPI providers, podcasts, local businesses, hiring signals, website enrichment, team pages, topic trends, trucking carriers.
- [`panda-web-security-tools`](https://github.com/pandadad0214/panda-web-security-tools) — Site, email and agent safety: SPF/DKIM/DMARC audits, AI/SEO readiness, website change monitoring, hidden AI instructions scanner.

Index / compatibility mega-server: [panda-federation-tools](https://github.com/pandadad0214/panda-federation-tools) (use only when you truly need every tool).

## TDQS standard

New tools join this domain only while the count stays in the 3–15 band. Descriptions follow the checklist in the umbrella repo. See [tdqs-standard](https://github.com/pandadad0214/panda-federation-tools) / project docs.

Built by Panda Federation. MIT licensed.

**Install** from [PyPI](https://pypi.org/project/panda-research-tools/) (needs [uv](https://docs.astral.sh/uv/) and a free [Apify token](https://console.apify.com/settings/integrations)):

```bash
uvx panda-research-tools@{{VERSION}}
```

- **Cursor / Claude / VS Code:** command `uvx`, args `["panda-research-tools"]`, env `APIFY_TOKEN`.
- Official MCP Registry name: `io.github.pandadad0214/panda-research-tools`.

### Added
- `topic_trends_tracker` (moved from leads so that domain stays in the 3–15 tool band). This server now has 8 tools.

### Changed
- Syncs with panda-federation-tools 1.8.0 (40 tools across four focused servers). Requires `panda-federation-tools>=1.8.0,<2`.

Full docs: [README](https://github.com/pandadad0214/panda-research-tools#readme).

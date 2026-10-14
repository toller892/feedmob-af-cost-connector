# FeedMob AF Cost Connector downloads

Public download of the **FeedMob AF Cost Connector 1.4.2** installer for Claude Desktop.

[Download the MCPB installer](https://github.com/toller892/feedmob-af-cost-connector/releases/download/connector-v1.4.2-preview/feedmob-af-cost-connector-1.4.2.mcpb)

This is the unchanged 1.4.2 preview installer previously distributed from `ai-team-publish/feedmob-appsflyer-reports-mcp`. Its extension interface and bundled guide are in Chinese; the tool descriptions are in English.

## Install

1. Download the `.mcpb` file.
2. In Claude Desktop, open **Settings > Extensions > Install extension** and select it.
3. Enter the dedicated **Connector Access Token** provided privately by your service administrator, then enable the extension.

No fm CLI or personal FeedMob Workspace/SSO Token is required. The installer connects to `https://af-reports.mcp.techmob.net/mcp`. Public downloads do not grant access to the service or its business data; a valid Connector Token is still required.

Example request:

> Query Binance AF Cost for 2026-10-01, reconcile it with FE gross spend, show Campaign/GEO differences and unmatched records, and generate Excel and CSV download links.

Currently supports Binance, UTC and USD. AF values come from validated server archives; FE is read when reconciling. Missing data and failed refreshes are reported explicitly. Exported reports use the existing server template, including Chinese labels. Downloads expire after 15 minutes.

## Verify the file

SHA-256:

```text
97381a2b9f43a07102cae0b9fe3fe002279d06ed824db2888a6d3201252e373b
```

File: `feedmob-af-cost-connector-1.4.2.mcpb` (2,497,338 bytes). The checksum matches the original release. Third-party dependency licenses remain bundled in the installer.

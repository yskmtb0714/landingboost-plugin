# LandingBoost for Claude

Give Claude eyes on your landing page. LandingBoost opens a public page in a browser at phone and desktop width, measures what a first-time visitor meets, and returns each problem with the exact current text and the change to make. Claude applies the change in your code, one at a time, and checks the live page again after you publish.

## Install

- **Claude (claude.ai, the desktop app, Cowork):** add LandingBoost from Claude's directory.
- **Claude Code:** run

  ```
  /plugin install landingboost --marketplace yskmtb0714/landingboost-plugin
  ```

- **Just the MCP server, in any client:** add `https://landingboost.app/mcp`. Setup for Claude Code, Cursor, Codex and VS Code: https://landingboost.app/mcp

## What's in this plugin

- **The LandingBoost MCP server** (`https://landingboost.app/mcp`): 13 tools for scans, fixes, re-checks and daily watching. It is a remote server; nothing is installed or run on your machine.
- **The `check-landing-page` skill**: teaches Claude the workflow. Find the page, scan it, apply the measured fixes one at a time, keep your facts, and re-check the live page after you deploy.

The plugin has no hooks, scripts or local commands.

## What it finds

Measured on the page, the same way on every site: two prices for the same plan, a cookie banner over the main button, plan cards with nothing to tap, broken links, visible errors, a page hidden from search, sideways scrolling on phones, and a slow first screen. Each one comes with the screenshot, the current text and the change.

## Try it

- "Scan example.com with LandingBoost and apply the top fix."
- "I published the change. Check the pricing page again."
- "What should I fix first across my sites?"
- "Watch my site and tell me when a price or a heading changes."

## Tools

| Tool | What it does |
| - | - |
| `scan_site` | Scan a website (up to 3 pages, phone and desktop). Counts toward your plan |
| `suggest_pages` | Suggest which pages to scan |
| `get_scan` | Scan status |
| `get_actions` | What to change, with the current and new text |
| `get_next_action` | The one thing to do next across your sites |
| `get_report` | The full report |
| `write_wording` | Write the new wording again when it failed |
| `recheck_page` | Check a page again after you publish (Pro and Lifetime) |
| `mark_done` | Mark an item done |
| `watch_site` | Re-read a site every day and report changes |
| `get_watches` | Watched sites and their changes |
| `get_sites` | Your sites |
| `list_scans` | Your scans |

## Account and data

- You need a LandingBoost account, free to start. The first call asks you to sign in with OAuth and press Allow; there is no token to copy. Free accounts get 1 scan a month with the full report.
- The plugin sends the URLs you ask it to scan, and the scan and item IDs it works with, to LandingBoost at `https://landingboost.app/mcp`. Nothing else leaves your machine through this plugin.
- LandingBoost reads public pages only and never changes your site. Your agent acts as you, on your own scans only, and you can disconnect it at any time under **MCP** in the LandingBoost app.
- Reports on the free plan are kept for 180 days; on paid plans, as long as your account exists. You can delete any report yourself.

Privacy policy: https://landingboost.app/privacy
Terms: https://landingboost.app/terms
Support: support@landingboost.app
Every client and every tool: https://landingboost.app/mcp

## License

MIT

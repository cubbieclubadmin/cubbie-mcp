# Cubbie Club Offers — MCP Server

A public, read-only [Model Context Protocol](https://modelcontextprotocol.io) server that lets AI agents discover current baby & kids brand discount codes and offers from [Cubbie Club](https://thecubbieclub.com).

- **Endpoint (Streamable HTTP):** `https://thecubbieclub.com/api/mcp`
- **Official MCP Registry:** `com.thecubbieclub/offers`
- **For LLM crawlers:** [`https://thecubbieclub.com/llms.txt`](https://thecubbieclub.com/llms.txt)

## Tools

| Tool | What it does |
|------|--------------|
| `search_offers(query)` | Find offers by brand name or keyword (e.g. `stroller`, `swim`, `snacks`). |
| `get_brand_offer(brand)` | The current offer for a specific brand. |
| `list_brands()` | Every brand with a live offer. |

Each result returns the discount, eligibility (new-customer flags), and a link to the brand's page on Cubbie Club. **Promo codes are never returned** — members unlock them free with a quick signup at the link.

## Connect

- **Claude:** add a custom connector for `https://thecubbieclub.com/api/mcp`.
- **ChatGPT / other MCP clients:** add the Streamable HTTP endpoint `https://thecubbieclub.com/api/mcp`.

## About

Cubbie Club is a free, parent-curated discovery network for baby & kids brand discounts. Learn more at [thecubbieclub.com](https://thecubbieclub.com).

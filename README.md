# Peru Import Export Data MCP

**Peru Customs Data: Importers, Suppliers & HS Codes.** Peru import export data for your AI assistant. Search Peru customs shipment records, find importers and foreign suppliers, and break down trade by HS code, partner country and counterparty company, through the Model Context Protocol.

An AI-native alternative to Peru trade data from Panjiva, ImportGenius, Volza, Seair, TradeInt and ExportGenius: ask in plain language instead of exporting spreadsheets.

The MCP connection is provided by [The Company Atlas](https://thecompanyatlas.com). This repository does not run a separate server.

## Connect

```
https://thecompanyatlas.com/mcp/trade/peru
```

Add this URL as a custom MCP connector in Claude, ChatGPT, Cursor, or any MCP-compatible client. Sign in with Google when prompted.

- Transport: Streamable HTTP
- Auth: Google OAuth (sign in once, stays authorized)
- Free accounts get 50 credits per calendar month
- Defaults to Peru: the server tells your AI to filter on `PE` unless you ask about another country

## Peru data coverage

- **Years:** 2019–2026
- **Records:** Import declarations: Peruvian importer, foreign supplier, origin country, HS code, goods description, value, quantity, port and date.
- **Country code:** `PE` (use `buyerCountry: "PE"` for imports into Peru)
- **Common products:** refined fuel (HS 2710), wheat (HS 1001), maize (HS 1005), earth-moving machinery (HS 8429)

## Notable traders in the data

Companies that appear most often in recent Peru records (by number of declaration lines, not value):

**Importers**

- Valero Perú
- Refinería La Pampilla
- Petroperú
- Cargill Americas Perú
- Bunge Perú
- Corporación Primax

## Example prompts

- *"Who are the top importers of wheat (HS 1001) into Peru?"*
- *"Which suppliers ship fuel to Petroperú?"*
- *"List Peruvian importers of mining equipment (HS 8429) in 2025"*
- *"What does Cargill Americas Perú import, by origin country?"*
- *"Show recent import shipments for Corporación Primax"*

## Tools

### Trade search

| Tool | Description |
|---|---|
| `Trade_search_trades` | Paginated customs shipment search: filter by HS code, buyer, seller, country, port, value and date range |
| `Trade_company_trade_volume_by_year` | Rank importers or exporters by declared value and line counts per year, with HS code and country filters |

### Trade analytics

| Tool | Description |
|---|---|
| `Trade_hs_code_breakdown` | For one company, import and export value by HS chapter, heading or subheading |
| `Trade_year_country_breakdown` | For one company, trade value by year and counterparty country |
| `Trade_partner_breakdown` | For one company, trade value by year and matched counterparty company |

### Company registry

| Tool | Description |
|---|---|
| `Company_search` | Search the global company registry by name or id, with optional country filter |
| `Company_get_by_id` | Full company profile by id |

## Keywords

Peru import data, Peru export data, Peru customs data, Peru shipment data, importers in Peru, Peru buyers and suppliers, HS code search, datos de importación Perú, importadores del Perú, comercio exterior, partida arancelaria

---
acting_count: 0
action_class_counts: {}
api_specs:
- filename: drillr-analyst-api-openapi.yml
  format: yaml
  label: drillr Public Data API Analyst API
  slug: drillr-analyst-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-analyst-api-openapi.yml
- filename: drillr-company-api-openapi.yml
  format: yaml
  label: drillr Public Data API Company API
  slug: drillr-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-company-api-openapi.yml
- filename: drillr-contract-api-openapi.yml
  format: yaml
  label: drillr Public Data API Contract API
  slug: drillr-contract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-contract-api-openapi.yml
- filename: drillr-earnings-api-openapi.yml
  format: yaml
  label: drillr Public Data API Earnings API
  slug: drillr-earnings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-earnings-api-openapi.yml
- filename: drillr-events-api-openapi.yml
  format: yaml
  label: drillr Public Data API Events API
  slug: drillr-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-events-api-openapi.yml
- filename: drillr-executives-api-openapi.yml
  format: yaml
  label: drillr Public Data API Executives API
  slug: drillr-executives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-executives-api-openapi.yml
- filename: drillr-filings-api-openapi.yml
  format: yaml
  label: drillr Public Data API Filings API
  slug: drillr-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-filings-api-openapi.yml
- filename: drillr-financials-api-openapi.yml
  format: yaml
  label: drillr Public Data API Financials API
  slug: drillr-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-financials-api-openapi.yml
- filename: drillr-ownership-api-openapi.yml
  format: yaml
  label: drillr Public Data API Ownership API
  slug: drillr-ownership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-ownership-api-openapi.yml
- filename: drillr-prices-api-openapi.yml
  format: yaml
  label: drillr Public Data API Prices API
  slug: drillr-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-prices-api-openapi.yml
- filename: drillr-signal-api-openapi.yml
  format: yaml
  label: drillr Public Data API Signal API
  slug: drillr-signal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-signal-api-openapi.yml
consequence_counts: {}
description: ''
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Drillr Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 0
overview: 'drillr Public Data API exposes 0 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: drillr Public Data API
provider_slug: drillr
slug: drillr-agentic-access
source_filename: drillr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: generated\nsource:\n- openapi/drillr-openapi.json\n- mcp/drillr-mcp-tools.json\n- https://drillr.ai/pricing\nsummary: >-\n  drillr is a fully read-only data and research API with no mutating operations, so\n  the agentic-access posture is uniform: every operation is a data read.\n  Consequence is bounded to credit spend, not to state change. The MCP tools all\n  declare readOnlyHint=true, destructiveHint=false, openWorldHint=false, confirming\n  a low-consequence agent surface.\ndefaults:\n  action_class: read\n  consequence: low\n  reversible: na           # nothing to reverse — no writes\n  escalation: none\n  token: account credential (REST X-API-KEY, or MCP OAuth session)\n  side_effects: none-beyond-credit-spend\nconsequence_model:\n  primary: spend\n  detail: >-\n    The only agent-visible consequence is credit consumption from the account's\n    shared pool. Fixed-rate tools cost 0.1-1 credit; company_search/company-discovery\n    is\
  \ usage-based (typically 3-5 credits, exact charge returned). ticker and schema\n    utilities are free. A 402 insufficient_credits fails closed and is not billed.\n  guidance: >-\n    An agent can call any endpoint safely without confirmation for correctness or\n    safety reasons; the only budgeting concern is credit spend on the metered tools\n    (company_search, signal tools, news_search). Resolve tickers first\n    (ticker_lookup / /tickers) — that step is free and avoids wasted metered calls.\noperation_classes:\n- class: read-free\n  token: account\n  consequence: none\n  operations: [publicDataV2Tickers]\n  mcp_tools: [ticker_lookup, get_table_schema, list_tables]\n- class: read-metered-low\n  token: account\n  consequence: spend (0.1-0.2 credit)\n  operations:\n  - publicDataV2Filings\n  - publicDataV2FilingSearch\n  - publicDataV2CompanyProfile\n  - publicDataV2IncomeStatements\n  - publicDataV2BalanceSheets\n  - publicDataV2CashFlowStatements\n  - publicDataV2FinancialMetricsSnapshot\n\
  \  - publicDataV2PricesHistorical\n  - publicDataV2PricesSnapshot\n  - publicDataV2EarningsCalendar\n  - publicDataV2EarningsCallSummary\n  - publicDataV2InsiderTrades\n  - publicDataV2InstitutionalHoldings\n  - publicDataV2Events\n  - publicDataV2EventsFinancings\n  - publicDataV2EventsDeals\n  - publicDataV2EventsExecutiveChanges\n  - publicDataV2EventsCorporateActions\n  - publicDataV2EventsOwnership\n  - publicDataV2AnalystConsensus\n  - publicDataV2AnalystRatings\n  - publicDataV2Executives\n  - publicDataV2ExecutiveCompensation\n  - publicDataV2NewsSearch\n  mcp_tools: [filing_list, filing_search, run_sql, news_search]\n- class: read-metered-usage\n  token: account\n  consequence: spend (usage-based, 3-5 credit typical) + daily cap\n  operations: [publicDataV2CompanyDiscovery, publicDataV2IndustryInflections, publicDataV2EnterpriseAiAdoption]\n  mcp_tools: [company_search, industry_inflections, ai_adoption]\n  note: >-\n    company_search / company-discovery is billed by actual research\
  \ work and is\n    additionally capped per day (Free 20, Plus 100, Ultra 500) as an abuse guard;\n    past the cap, calls are declined and not charged.\nno_write_surface: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/agentic-access/drillr-agentic-access.yml
summary_line: 0 operations
tags:
- Financial Data
- Stocks
- SEC Filings
- Fundamentals
- Earnings
- Ownership
- Corporate Events
- Analyst Ratings
- news-signals
- MCP
- agent-native
---

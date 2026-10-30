---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 27
api_specs:
- filename: alphagrowth-io-alphagrowth-api-api-openapi.yml
  format: yaml
  label: AlphaGrowth AlphaGrowth API
  slug: alphagrowth-io-alphagrowth-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphagrowth-io/openapi/alphagrowth-io-alphagrowth-api-api-openapi.yml
- filename: alphagrowth-io-chains-api-openapi.yml
  format: yaml
  label: AlphaGrowth Chains API
  slug: alphagrowth-io-chains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphagrowth-io/openapi/alphagrowth-io-chains-api-openapi.yml
- filename: alphagrowth-io-dao-treasuries-api-openapi.yml
  format: yaml
  label: AlphaGrowth Dao Treasuries API
  slug: alphagrowth-io-dao-treasuries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphagrowth-io/openapi/alphagrowth-io-dao-treasuries-api-openapi.yml
- filename: alphagrowth-io-fees-api-openapi.yml
  format: yaml
  label: AlphaGrowth Fees API
  slug: alphagrowth-io-fees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphagrowth-io/openapi/alphagrowth-io-fees-api-openapi.yml
- filename: alphagrowth-io-funding-rounds-api-openapi.yml
  format: yaml
  label: AlphaGrowth Funding Rounds API
  slug: alphagrowth-io-funding-rounds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphagrowth-io/openapi/alphagrowth-io-funding-rounds-api-openapi.yml
- filename: alphagrowth-io-health-api-openapi.yml
  format: yaml
  label: AlphaGrowth Health API
  slug: alphagrowth-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphagrowth-io/openapi/alphagrowth-io-health-api-openapi.yml
- filename: alphagrowth-io-investors-api-openapi.yml
  format: yaml
  label: AlphaGrowth Investors API
  slug: alphagrowth-io-investors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphagrowth-io/openapi/alphagrowth-io-investors-api-openapi.yml
- filename: alphagrowth-io-llms-full-txt-api-openapi.yml
  format: yaml
  label: AlphaGrowth Llms Full.txt API
  slug: alphagrowth-io-llms-full-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphagrowth-io/openapi/alphagrowth-io-llms-full-txt-api-openapi.yml
- filename: alphagrowth-io-llms-txt-api-openapi.yml
  format: yaml
  label: AlphaGrowth Llms.txt API
  slug: alphagrowth-io-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphagrowth-io/openapi/alphagrowth-io-llms-txt-api-openapi.yml
- filename: alphagrowth-io-mcp-api-openapi.yml
  format: yaml
  label: AlphaGrowth MCP API
  slug: alphagrowth-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphagrowth-io/openapi/alphagrowth-io-mcp-api-openapi.yml
- filename: alphagrowth-io-projects-api-openapi.yml
  format: yaml
  label: AlphaGrowth Projects API
  slug: alphagrowth-io-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphagrowth-io/openapi/alphagrowth-io-projects-api-openapi.yml
- filename: alphagrowth-io-rankings-api-openapi.yml
  format: yaml
  label: AlphaGrowth Rankings API
  slug: alphagrowth-io-rankings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphagrowth-io/openapi/alphagrowth-io-rankings-api-openapi.yml
- filename: alphagrowth-io-search-history-api-openapi.yml
  format: yaml
  label: AlphaGrowth Search History API
  slug: alphagrowth-io-search-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphagrowth-io/openapi/alphagrowth-io-search-history-api-openapi.yml
- filename: alphagrowth-io-treasury-companies-api-openapi.yml
  format: yaml
  label: AlphaGrowth Treasury Companies API
  slug: alphagrowth-io-treasury-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphagrowth-io/openapi/alphagrowth-io-treasury-companies-api-openapi.yml
consequence_counts:
  read: 27
  safety-critical: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Alphagrowth Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /mcp
operation_count: 29
overview: 'AlphaGrowth exposes 29 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read, 1 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AlphaGrowth
provider_slug: alphagrowth-io
slug: alphagrowth-io-agentic-access
source_filename: alphagrowth-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/alphagrowth-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 27\n    acting: 2\n  by_consequence:\n    read: 27\n    safety-critical: 1\n    write: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1\n  method: get\n  operationId: dataApiIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chains\n  method: get\n  operationId: chains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chains/metrics\n\
  \  method: get\n  operationId: chain_metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/dao-treasuries\n  method: get\n  operationId: dao_treasuries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/dao-treasuries/history\n  method: get\n  operationId: dao_treasury_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/dao-treasuries/holdings-history\n  method: get\n  operationId: dao_holdings_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/dao-treasuries/snapshot\n  method: get\n  operationId: dao_treasury_snapshot\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/dao-treasuries/{id}\n  method: get\n  operationId: dao_treasury\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fees\n  method: get\n  operationId: fees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/funding-rounds\n  method: get\n  operationId: recent_funding_rounds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/investors/profile\n  method: get\n  operationId: investor_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/investors/top\n  method: get\n  operationId: top_investors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/projects/community\n  method: get\n  operationId: project_community\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/projects/find\n  method: get\n  operationId: find_projects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/projects/funding\n  method: get\n  operationId: project_funding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/projects/metrics\n  method: get\n  operationId: project_metrics\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/rankings/projects\n  method: get\n  operationId: rank_projects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/treasury-companies\n  method: get\n  operationId: treasury_companies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dao-treasuries/export.csv\n  method: get\n  operationId: daoTreasuriesExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fees/export.csv\n  method: get\n  operationId: feesExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms-full.txt\n  method: get\n  operationId: llmsFull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: llms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: get\n  operationId: mcpStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: delete\n  operationId: mcpTerminate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search-history/export.csv\n  method: get\n  operationId: searchHistoryExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search-history/transcripts.zip\n  method: get\n  operationId: searchHistoryTranscripts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /{page}.md\n  method: get\n  operationId: pageMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/alphagrowth-io/agentic-access/alphagrowth-io-agentic-access.yml
summary_line: 29 operations · 2 acting · 1 human-in-the-loop
tags:
- Company
- Crypto
- DeFi
- DataAnalytics
- Finance
---

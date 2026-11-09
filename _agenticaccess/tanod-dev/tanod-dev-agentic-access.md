---
acting_count: 288
action_class_counts:
  acting: 288
  connected: 88
api_specs:
- filename: tanod-dev-agentscan-api-openapi.yml
  format: yaml
  label: tanod-dev Agentscan API
  slug: tanod-dev-agentscan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tanod-dev/openapi/tanod-dev-agentscan-api-openapi.yml
- filename: tanod-dev-chainpeek-api-openapi.yml
  format: yaml
  label: tanod-dev Chainpeek API
  slug: tanod-dev-chainpeek-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tanod-dev/openapi/tanod-dev-chainpeek-api-openapi.yml
- filename: tanod-dev-dnspeek-api-openapi.yml
  format: yaml
  label: tanod-dev Dnspeek API
  slug: tanod-dev-dnspeek-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tanod-dev/openapi/tanod-dev-dnspeek-api-openapi.yml
- filename: tanod-dev-findpeek-api-openapi.yml
  format: yaml
  label: tanod-dev Findpeek API
  slug: tanod-dev-findpeek-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tanod-dev/openapi/tanod-dev-findpeek-api-openapi.yml
- filename: tanod-dev-imagepeek-api-openapi.yml
  format: yaml
  label: tanod-dev Imagepeek API
  slug: tanod-dev-imagepeek-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tanod-dev/openapi/tanod-dev-imagepeek-api-openapi.yml
- filename: tanod-dev-mlpeek-api-openapi.yml
  format: yaml
  label: tanod-dev Mlpeek API
  slug: tanod-dev-mlpeek-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tanod-dev/openapi/tanod-dev-mlpeek-api-openapi.yml
- filename: tanod-dev-pactlint-api-openapi.yml
  format: yaml
  label: tanod-dev Pactlint API
  slug: tanod-dev-pactlint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tanod-dev/openapi/tanod-dev-pactlint-api-openapi.yml
- filename: tanod-dev-pdfpeek-api-openapi.yml
  format: yaml
  label: tanod-dev Pdfpeek API
  slug: tanod-dev-pdfpeek-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tanod-dev/openapi/tanod-dev-pdfpeek-api-openapi.yml
- filename: tanod-dev-sitepeek-api-openapi.yml
  format: yaml
  label: tanod-dev Sitepeek API
  slug: tanod-dev-sitepeek-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tanod-dev/openapi/tanod-dev-sitepeek-api-openapi.yml
- filename: tanod-dev-skypeek-api-openapi.yml
  format: yaml
  label: tanod-dev Skypeek API
  slug: tanod-dev-skypeek-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tanod-dev/openapi/tanod-dev-skypeek-api-openapi.yml
- filename: tanod-dev-toolsniff-api-openapi.yml
  format: yaml
  label: tanod-dev Toolsniff API
  slug: tanod-dev-toolsniff-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tanod-dev/openapi/tanod-dev-toolsniff-api-openapi.yml
- filename: tanod-dev-txpeek-api-openapi.yml
  format: yaml
  label: tanod-dev Txpeek API
  slug: tanod-dev-txpeek-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tanod-dev/openapi/tanod-dev-txpeek-api-openapi.yml
- filename: tanod-dev-utilpeek-api-openapi.yml
  format: yaml
  label: tanod-dev Utilpeek API
  slug: tanod-dev-utilpeek-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tanod-dev/openapi/tanod-dev-utilpeek-api-openapi.yml
- filename: tanod-dev-weatherpeek-api-openapi.yml
  format: yaml
  label: tanod-dev Weatherpeek API
  slug: tanod-dev-weatherpeek-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tanod-dev/openapi/tanod-dev-weatherpeek-api-openapi.yml
consequence_counts:
  physical: 21
  read: 88
  safety-critical: 7
  write: 260
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 7
kind: agentic-access
layout: agentic-access
method: generated
name: Tanod Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/chain/approvals
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/chain/solana/token-safety
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/chain/token-safety
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/scan/package
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/scan/package
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/vehicle/recalls
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/web/agent-readiness/fix
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/chain/address-poisoning
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/chain/bolt11/decode
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/chain/counterparties
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/chain/drain-check
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/chain/erc20-transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/chain/pre-trade-check
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/chain/token-trades
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/chain/transfer-fees
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/chain/transfer-preflight
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/check/address
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/check/address
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/einvoice/peppol-lookup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/pdf/extract-pages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/pdf/extract-pages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/pdf/reorder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/pdf/reorder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/solana/reward-yield
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/solana/token-trades
operation_count: 376
overview: 'tanod-dev exposes 376 API operations that an AI agent could call, of which 288 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 88 read, 260 write, 21 physical, and 7 safety-critical.


  7 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: tanod-dev
provider_slug: tanod-dev
slug: tanod-dev-agentic-access
source_filename: tanod-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/agents.json, openapi/chain.json, openapi/docs.json, openapi/finance.json, openapi/images.json,\n  openapi/ml.json, openapi/openapi.json, openapi/security.json, openapi/sky.json, openapi/text.json,\n  openapi/util.json, openapi/web.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 376\n  by_action_class:\n    connected: 88\n    acting: 288\n  by_consequence:\n    read: 88\n    safety-critical: 7\n    physical: 21\n    write: 260\n  human_in_the_loop_required: 7\noperations:\n- path: /v1/x402/pulse\n  method: get\n  operationId: get_x402_bazaar_pulse_today_no_params\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/x402/pulse\n  method: post\n  operationId: get_x402_bazaar_pulse_new_listings_demand_gaps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/uptime\n  method: post\n  operationId: get_x402_mcp_endpoint_uptime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/uptime/bulk\n  method: post\n  operationId: get_x402_mcp_endpoint_uptime_bulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scan/package\n  method: post\n  operationId: scan_mcp_server_agent_skill_package\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/x402/payment-status\n  method: post\n  operationId: get_x402_payment_authorization_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/receipt-check\n  method: post\n  operationId: check_x402_payment_receipt\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/well-known-file\n  method: post\n  operationId: build_x402_well_known_file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/edge-check\n  method: post\n  operationId: check_x402_edge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/price-benchmark\n  method: post\n  operationId: x402_price_benchmark\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/pay-test\n  method: post\n  operationId: x402_ping\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/preflight\n  method: post\n  operationId: check_x402_endpoint_before_paying\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/seller-report\n  method: post\n  operationId: x402_seller_report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/listing-audit\n\
  \  method: post\n  operationId: x402_listing_audit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mcp/check\n  method: post\n  operationId: check_mcp_server\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/web/agent-readiness\n  method: post\n  operationId: check_agent_readiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/x402/facilitators\n  method: post\n  operationId: get_x402_facilitator_support_and_changes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mcp/listing-audit\n  method: post\n  operationId: audit_mcp_listings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mcp/list-preflight\n  method: post\n  operationId: preflight_mcp_listing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/repeat-demand\n  method: post\n  operationId: get_x402_endpoints_with_repeat_paying_demand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/clients\n  method: post\n  operationId: identify_x402_client_by_user_agent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/web/agent-traffic\n  method: post\n  operationId: analyze_ai_agent_traffic_in_web_server_logs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apify/rules-check\n  method: post\n  operationId: check_apify_store_rules_for_actors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/web/agent-readiness/fix\n  method: post\n  operationId: generate_agent_ready_files_for_a_site\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/x402/price-consistency\n  method: post\n\
  \  operationId: x402_price_consistency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/query\n  method: post\n  operationId: search_x402_mcp_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/history\n  method: post\n  operationId: get_x402_mcp_record_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/export\n  method: post\n  operationId: export_x402_mcp_index\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/delta\n  method: post\n  operationId: agent_index_delta\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/bulk\n  method: post\n  operationId: download_x402_mcp_index_snapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/defi/funding\n  method: post\n  operationId: get_perp_funding_rates_hyperliquid\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/check/address\n  method: post\n  operationId: check_address_risk\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chain/ens\n  method: post\n  operationId: resolve_ens_name\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chain/calldata\n  method: post\n  operationId: decode_calldata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chain/token\n  method: post\n  operationId: get_token_info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chain/balance\n  method: post\n  operationId: get_wallet_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/gas\n  method: post\n  operationId: get_gas_price\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/block\n\
  \  method: post\n  operationId: get_latest_block\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/price\n  method: post\n  operationId: get_token_price\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chain/tx\n  method: post\n  operationId: get_transaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/nft\n  method: post\n  operationId: lookup_nft_owner_token_uri\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chain/allowance\n  method: post\n  operationId: check_erc20_allowance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chain/portfolio\n  method: post\n  operationId: get_wallet_portfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/quote\n  method: post\n  operationId: get_swap_quote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sanctions\n  method: post\n  operationId: screen_crypto_address_ofac_sanctions\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chain/block-at\n  method: post\n  operationId: find_block_by_timestamp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/proxy\n  method: post\n  operationId: detect_proxy_contract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chain/ens-records\n  method: post\n  operationId: get_ens_records\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/logs\n  method: post\n  operationId: decode_transaction_event_logs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chain/candles\n  method: post\n  operationId: get_crypto_ohlcv_price_candles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/nonce\n  method: post\n  operationId: get_account_transaction_count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/receipt\n  method: post\n  operationId: get_transaction_receipt_gas_status_logs_count\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/events\n  method: post\n  operationId: query_contract_event_logs_by_block_range\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/call\n  method: post\n  operationId: call_smart_contract_read_only\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chain/estimate-gas\n  method: post\n  operationId: estimate_transaction_gas\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chain/storage\n  method: post\n  operationId: read_contract_storage_slot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chain/erc1155-balance\n  method: post\n  operationId: get_erc1155_token_balance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chain/info\n  method: post\n  operationId: get_blockchain_chain_id_head_age_gas_price\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/erc20-transfers\n  method: post\n  operationId: list_erc20_token_transfers_for_address\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chain/block-number\n  method: post\n  operationId: get_latest_block_number_and_age\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chain/code\n  method: post\n  operationId: get_contract_bytecode_hash_proxy_7702\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/total-supply\n  method: post\n  operationId: get_erc20_total_supply\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/nft-owner\n  method: post\n  operationId: get_erc721_owner_and_token_uri\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/solana/balance\n  method: post\n  operationId: get_solana_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/solana/tokens\n\
  \  method: post\n  operationId: get_solana_token_balances\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/solana/transaction\n  method: post\n  operationId: get_solana_transaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/solana/signatures\n  method: post\n  operationId: list_solana_transaction_signatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/solana/account\n  method: post\n  operationId: get_solana_account_info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/solana/token-info\n  method: post\n  operationId: get_solana_token_mint_info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/defi/perps\n  method: post\n  operationId: list_perp_markets_hyperliquid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/gas/base\n  method: get\n  operationId: get_base_gas_price\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/docs/to-markdown\n  method: post\n  operationId: convert_pdf_to_markdown\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/tables\n  method: post\n  operationId: extract_tables_from_pdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/bank-statement\n  method: post\n  operationId: convert_bank_statement_to_csv\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/to-docx\n  method: post\n  operationId: convert_pdf_to_word\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/merge\n  method: post\n  operationId: merge_pdf_files\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf\n  method: post\n  operationId: pdf_to_text\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ocr\n  method: post\n  operationId:\
  \ image_to_text\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/split\n  method: post\n  operationId: split_pdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/extract-pages\n  method: post\n  operationId: extract_pdf_pages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/pdf/remove-pages\n  method: post\n  operationId: remove_pdf_pages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/rotate\n  method: post\n  operationId: rotate_pdf_pages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/compress\n  method: post\n  operationId: compress_pdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/to-images\n  method: post\n  operationId: convert_pdf_to_images\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/rasterize\n  method: post\n  operationId: flatten_pdf_to_image_only\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/from-images\n  method: post\n  operationId: convert_images_to_pdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/watermark\n  method: post\n  operationId: add_watermark_to_pdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/page-numbers\n  method: post\n  operationId: add_pdf_page_numbers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/protect\n  method: post\n  operationId: password_protect_pdf\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/unlock\n  method: post\n  operationId: unlock_pdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/metadata\n  method: post\n  operationId: edit_pdf_metadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/html-to-pdf\n  method: post\n  operationId: url_to_pdf\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/ocr\n  method: post\n  operationId: ocr_pdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/inspect\n  method: post\n  operationId: inspect_pdf_document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/reorder\n  method:\
  \ post\n  operationId: reorder_pdf_pages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/crop\n  method: post\n  operationId: crop_pdf_pages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/resize\n  method: post\n  operationId: resize_pdf_pages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/outline\n  method: post\n  operationId: read_pdf_bookmarks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/set-outline\n  method: post\n  operationId: write_pdf_bookmarks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/form-fields\n  method: post\n  operationId: list_pdf_form_fields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/pdf/fill-form\n  method: post\n  operationId: fill_pdf_form\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/flatten\n  method: post\n  operationId: flatten_pdf_forms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf/repair\n  method: post\n  operationId: repair_damaged_pdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (117 KB total) ---\n# Full source: https://artifacts.apis.io/tanod-dev/agentic-access/tanod-dev-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/tanod-dev/agentic-access/tanod-dev-agentic-access.yml
summary_line: 376 operations · 288 acting · 7 human-in-the-loop
tags:
- Artificial Intelligence
- MCP
- Tools
- Finance
- Monitoring
---

---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 80
api_specs:
- filename: satoshidata-ai-batch-api-openapi.yml
  format: yaml
  label: satoshidata-ai Batch API
  slug: satoshidata-ai-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-batch-api-openapi.yml
- filename: satoshidata-ai-billing-api-openapi.yml
  format: yaml
  label: satoshidata-ai Billing API
  slug: satoshidata-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-billing-api-openapi.yml
- filename: satoshidata-ai-chain-api-openapi.yml
  format: yaml
  label: satoshidata-ai Chain API
  slug: satoshidata-ai-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-chain-api-openapi.yml
- filename: satoshidata-ai-community-api-openapi.yml
  format: yaml
  label: satoshidata-ai Community API
  slug: satoshidata-ai-community-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-community-api-openapi.yml
- filename: satoshidata-ai-discovery-api-openapi.yml
  format: yaml
  label: satoshidata-ai Discovery API
  slug: satoshidata-ai-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-discovery-api-openapi.yml
- filename: satoshidata-ai-entities-api-openapi.yml
  format: yaml
  label: satoshidata-ai Entities API
  slug: satoshidata-ai-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-entities-api-openapi.yml
- filename: satoshidata-ai-feedback-api-openapi.yml
  format: yaml
  label: satoshidata-ai Feedback API
  slug: satoshidata-ai-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-feedback-api-openapi.yml
- filename: satoshidata-ai-health-api-openapi.yml
  format: yaml
  label: satoshidata-ai Health API
  slug: satoshidata-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-health-api-openapi.yml
- filename: satoshidata-ai-labels-api-openapi.yml
  format: yaml
  label: satoshidata-ai Labels API
  slug: satoshidata-ai-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-labels-api-openapi.yml
- filename: satoshidata-ai-market-api-openapi.yml
  format: yaml
  label: satoshidata-ai Market API
  slug: satoshidata-ai-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-market-api-openapi.yml
- filename: satoshidata-ai-metrics-api-openapi.yml
  format: yaml
  label: satoshidata-ai Metrics API
  slug: satoshidata-ai-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-metrics-api-openapi.yml
- filename: satoshidata-ai-risk-api-openapi.yml
  format: yaml
  label: satoshidata-ai Risk API
  slug: satoshidata-ai-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-risk-api-openapi.yml
- filename: satoshidata-ai-sanctions-api-openapi.yml
  format: yaml
  label: satoshidata-ai Sanctions API
  slug: satoshidata-ai-sanctions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-sanctions-api-openapi.yml
- filename: satoshidata-ai-timestamping-api-openapi.yml
  format: yaml
  label: satoshidata-ai Timestamping API
  slug: satoshidata-ai-timestamping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-timestamping-api-openapi.yml
- filename: satoshidata-ai-wallets-api-openapi.yml
  format: yaml
  label: satoshidata-ai Wallets API
  slug: satoshidata-ai-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/satoshidata-ai/openapi/satoshidata-ai-wallets-api-openapi.yml
consequence_counts:
  physical: 4
  read: 80
  safety-critical: 1
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Satoshidata Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/batch/trust-safety
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/checkout/{checkout_id}/refresh
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/community/reports
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/tx/verify
operation_count: 96
overview: 'satoshidata-ai exposes 96 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 80 read, 11 write, 4 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: satoshidata-ai
provider_slug: satoshidata-ai
slug: satoshidata-ai-agentic-access
source_filename: satoshidata-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/satoshidata-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 96\n  by_action_class:\n    connected: 80\n    acting: 16\n  by_consequence:\n    read: 80\n    physical: 4\n    write: 11\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/health\n  method: get\n  operationId: api_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health/full\n  method: get\n  operationId: api_health_full\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/capabilities\n  method: get\n  operationId: capabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/beta-status\n  method: get\n  operationId: beta_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sanctions/ofac/compliance-tier\n  method: get\n  operationId: sanctions_ofac_compliance_tier_v1_sanctions_ofac_compliance_tier_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sanctions/ofac/coverage\n  method: get\n  operationId: sanctions_ofac_coverage_v1_sanctions_ofac_coverage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/wallets\n  method: get\n  operationId: wallets_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallets/{address}/trust-safety\n  method: get\n  operationId: wallet_trust_safety\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallets/{address}/surveillance-status\n  method: get\n  operationId: wallet_surveillance_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallets/{address}/flow-graph\n  method: get\n  operationId: wallet_flow_graph\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallets/{address}/overview\n  method: get\n  operationId:\
  \ wallet_overview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallets/{address}/transactions\n  method: get\n  operationId: wallet_transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallets/{address}/pnl\n  method: get\n  operationId: wallet_pnl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallets/{address}/dashboard\n  method: get\n  operationId: wallet_dashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallets/{address}/balance-history\n  method: get\n  operationId: wallet_balance_history\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/community/reports\n  method: post\n  operationId: community_report_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/community/reports/{report_id}/status\n  method: get\n  operationId: community_report_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/qr\n  method: get\n  operationId: qr_code_png\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/community/reports/{report_id}/vote\n\
  \  method: post\n  operationId: community_report_vote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/community/reports/{address}\n  method: get\n  operationId: community_reports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feedback\n  method: post\n  operationId: submit_feedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/wallets/{address}/summary\n  method: get\n  operationId: wallet_summary\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallets/{address}/detail\n  method: get\n  operationId: wallet_detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallets/{address}/contributors\n  method: get\n  operationId: wallet_contributors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallets/{address}/intelligence\n  method: get\n  operationId: address_intelligence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallets/{address}/risk-signals\n  method: get\n  operationId: address_risk\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/address/{address}/risk-signals\n  method: get\n  operationId: address_risk_signals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallets/{address}/evidence-pack\n  method: get\n  operationId: address_evidence_pack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/risk-check/{address}\n  method: get\n  operationId: risk_check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/risk-check/batch\n  method: post\n  operationId: risk_check_batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/wallets/{address}/risk-exposure\n  method: get\n  operationId: wallet_risk_exposure_oracle_v1_wallets__address__risk_exposure_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallets/{address}/sanctions-exposure\n  method: get\n  operationId: wallet_sanctions_exposure_v1_wallets__address__sanctions_exposure_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch/trust-safety\n  method: post\n  operationId: batch_trust_safety\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/batch/summary\n  method: post\n  operationId: batch_summary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch/intelligence\n  method: post\n  operationId: batch_intelligence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch/risk-signals\n  method: post\n  operationId: batch_risk_signals\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/addresses/risk-signals\n  method: post\n  operationId: addresses_batch_risk_signals\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/timestamp\n  method: post\n  operationId: timestamp_hash\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/timestamp/quote\n  method: get\n  operationId: timestamp_quote\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/timestamp/{hash_hex}\n  method: get\n  operationId: timestamp_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/timestamp/{hash_hex}/proof\n  method: get\n  operationId: timestamp_proof\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/timestamp/verify\n  method: post\n  operationId: verify_timestamp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/fees/recommended\n  method:\
  \ get\n  operationId: fees_recommended\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mempool/stats\n  method: get\n  operationId: mempool_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mempool/fee-distribution\n  method: get\n  operationId: mempool_fee_distribution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mempool/tx/{txid}\n  method: get\n  operationId: mempool_tx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/network/mempool/stress\n  method: get\n  operationId: mempool_stress\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/blocks/{height_or_hash}\n  method: get\n  operationId: block_detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/recent-blocks\n  method: get\n  operationId: recent_blocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/projected-blocks\n  method: get\n  operationId: projected_blocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities/categories\n  method: get\n  operationId: entity_categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities/list\n\
  \  method: get\n  operationId: entity_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities/directory\n  method: get\n  operationId: entity_directory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities/{entity_name}/activity\n  method: get\n  operationId: entity_recent_activity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities/{entity_name}\n  method: get\n  operationId: entity_lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/price\n  method: get\n  operationId: bitcoin_price\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/price-history\n  method: get\n  operationId: market_price_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/fx-history\n  method: get\n  operationId: market_fx_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/network/summary\n  method: get\n  operationId: network_intelligence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/whale-alerts\n  method: get\n  operationId: whale_alerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/pulse/whales\n  method: get\n  operationId: pulse_whales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pulse/dormant\n  method: get\n  operationId: pulse_dormant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pulse/consolidations\n  method: get\n  operationId: pulse_consolidations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pulse/summary\n  method: get\n  operationId: pulse_summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/dormancy-flushes\n  method: get\n  operationId: dormancy_flushes\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/whale-alerts/labeled\n  method: get\n  operationId: whale_alerts_labeled\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exchange/flows/summary\n  method: get\n  operationId: exchange_flows_summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pools/list\n  method: get\n  operationId: pool_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pools/{pool_name}\n  method: get\n  operationId: pool_detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /v1/dormancy/whale-wakeups\n  method: get\n  operationId: dormancy_whale_wakeups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dormancy/watchlist\n  method: get\n  operationId: dormancy_watchlist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dormancy/weekly.json\n  method: get\n  operationId: dormancy_weekly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dormancy/weekly.md\n  method: get\n  operationId: dormancy_weekly_markdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tx/{txid}/status\n  method: get\n  operationId:\
  \ tx_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tx/{txid}/op-return\n  method: get\n  operationId: op_return_decode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tx/{txid}\n  method: get\n  operationId: tx_lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tx/verify\n  method: post\n  operationId: tx_verify\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/tx/broadcast\n  method: post\n  operationId: tx_broadcast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/exchange/flows\n  method: get\n  operationId: exchange_flows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/miner/flows\n  method: get\n  operationId: miner_flows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/awakenings\n  method: get\n  operationId: chain_awakenings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/chain/dormant-movements\n  method: get\n  operationId: dormant_movements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/dormant-alerts\n  method: get\n  operationId: dormant_alerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/activity-feed\n  method: get\n  operationId: activity_feed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/supply-distribution\n  method: get\n  operationId: supply_distribution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/onchain\n  method: get\n  operationId: onchain_stats\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/catalog\n  method: get\n  operationId: billing_catalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/checkout\n  method: post\n  operationId: billing_checkout_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/redeem\n  method: post\n  operationId: billing_redeem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/checkout/{checkout_id}\n  method: get\n  operationId: billing_checkout_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/checkout/{checkout_id}/refresh\n  method: post\n  operationId: billing_checkout_refresh\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/agent-card.json\n  method: get\n  operationId: agent_card_discovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /.well-known/x402\n  method: get\n  operationId: x402_discovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp.json\n  method: get\n  operationId: mcp_discovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/glama.json\n  method: get\n  operationId: glama_discovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/labels/search\n  method: get\n  operationId: label_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/satoshidata-ai/agentic-access/satoshidata-ai-agentic-access.yml
summary_line: 96 operations · 16 acting · 1 human-in-the-loop
tags:
- Bitcoin
- Artificial Intelligence
- Finance
- Chain-Intelligence
- Company
---

---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 4
api_specs:
- filename: anchor-x402-anchor-api-openapi.yml
  format: yaml
  label: anchor-x402 Anchor API
  slug: anchor-x402-anchor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-anchor-api-openapi.yml
- filename: anchor-x402-attest-api-openapi.yml
  format: yaml
  label: anchor-x402 Attest API
  slug: anchor-x402-attest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-attest-api-openapi.yml
- filename: anchor-x402-aura-api-openapi.yml
  format: yaml
  label: anchor-x402 Aura API
  slug: anchor-x402-aura-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-aura-api-openapi.yml
- filename: anchor-x402-decode-api-openapi.yml
  format: yaml
  label: anchor-x402 Decode API
  slug: anchor-x402-decode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-decode-api-openapi.yml
- filename: anchor-x402-grade-api-openapi.yml
  format: yaml
  label: anchor-x402 Grade API
  slug: anchor-x402-grade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-grade-api-openapi.yml
- filename: anchor-x402-health-api-openapi.yml
  format: yaml
  label: anchor-x402 Health API
  slug: anchor-x402-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-health-api-openapi.yml
- filename: anchor-x402-intel-api-openapi.yml
  format: yaml
  label: anchor-x402 Intel API
  slug: anchor-x402-intel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-intel-api-openapi.yml
- filename: anchor-x402-investigate-api-openapi.yml
  format: yaml
  label: anchor-x402 Investigate API
  slug: anchor-x402-investigate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-investigate-api-openapi.yml
- filename: anchor-x402-ledger-api-openapi.yml
  format: yaml
  label: anchor-x402 Ledger API
  slug: anchor-x402-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-ledger-api-openapi.yml
- filename: anchor-x402-oracle-api-openapi.yml
  format: yaml
  label: anchor-x402 Oracle API
  slug: anchor-x402-oracle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-oracle-api-openapi.yml
- filename: anchor-x402-parse-api-openapi.yml
  format: yaml
  label: anchor-x402 Parse API
  slug: anchor-x402-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-parse-api-openapi.yml
- filename: anchor-x402-price-api-openapi.yml
  format: yaml
  label: anchor-x402 Price API
  slug: anchor-x402-price-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-price-api-openapi.yml
- filename: anchor-x402-resolve-api-openapi.yml
  format: yaml
  label: anchor-x402 Resolve API
  slug: anchor-x402-resolve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-resolve-api-openapi.yml
- filename: anchor-x402-roast-api-openapi.yml
  format: yaml
  label: anchor-x402 Roast API
  slug: anchor-x402-roast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-roast-api-openapi.yml
- filename: anchor-x402-roll-api-openapi.yml
  format: yaml
  label: anchor-x402 Roll API
  slug: anchor-x402-roll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-roll-api-openapi.yml
- filename: anchor-x402-screen-api-openapi.yml
  format: yaml
  label: anchor-x402 Screen API
  slug: anchor-x402-screen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-screen-api-openapi.yml
- filename: anchor-x402-tldr-api-openapi.yml
  format: yaml
  label: anchor-x402 Tldr API
  slug: anchor-x402-tldr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-tldr-api-openapi.yml
- filename: anchor-x402-feedback-api-openapi.yml
  format: yaml
  label: anchor-x402 Feedback API
  slug: anchor-x402-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-feedback-api-openapi.yml
consequence_counts:
  read: 4
  safety-critical: 2
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Anchor X402 Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/investigate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/ledger/report
operation_count: 24
overview: 'anchor-x402 exposes 24 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 18 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: anchor-x402
provider_slug: anchor-x402
slug: anchor-x402-agentic-access
source_filename: anchor-x402-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/anchor-x402-anchor-api-openapi.yml, openapi/anchor-x402-attest-api-openapi.yml,\n  openapi/anchor-x402-aura-api-openapi.yml, openapi/anchor-x402-decode-api-openapi.yml, openapi/anchor-x402-feedback-api-openapi.yml,\n  openapi/anchor-x402-grade-api-openapi.yml, openapi/anchor-x402-health-api-openapi.yml, openapi/anchor-x402-intel-api-openapi.yml,\n  openapi/anchor-x402-investigate-api-openapi.yml, openapi/anchor-x402-ledger-api-openapi.yml,\n  openapi/anchor-x402-oracle-api-openapi.yml, openapi/anchor-x402-parse-api-openapi.yml, openapi/anchor-x402-price-api-openapi.yml,\n  openapi/anchor-x402-resolve-api-openapi.yml, openapi/anchor-x402-roast-api-openapi.yml, openapi/anchor-x402-roll-api-openapi.yml,\n  openapi/anchor-x402-screen-api-openapi.yml, openapi/anchor-x402-tldr-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting\
  \ point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    acting: 20\n    connected: 4\n  by_consequence:\n    write: 18\n    read: 4\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v1/anchor\n  method: post\n  operationId: anchor_v1_anchor_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/attest\n  method: post\n  operationId: attest_v1_attest_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/attest/verify\n  method: post\n  operationId: attest_verify_v1_attest_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/aura\n  method: post\n  operationId: aura_v1_aura_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/decode/tx\n  method: post\n  operationId: decode_tx_v1_decode_tx_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/decode/calldata\n  method: post\n  operationId: decode_calldata_v1_decode_calldata_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/feedback\n  method: get\n  operationId: feedback_help_v1_feedback_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feedback\n  method: post\n  operationId: feedback_v1_feedback_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /v1/grade\n  method: post\n  operationId: grade_v1_grade_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/intel/wallet\n  method: post\n  operationId: intel_wallet_post_v1_intel_wallet_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/investigate\n\
  \  method: post\n  operationId: investigate_dispatch_v1_investigate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/investigate/status/{job_id}\n  method: get\n  operationId: investigate_status_v1_investigate_status__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ledger/summary\n  method: post\n  operationId: ledger_summary_v1_ledger_summary_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /v1/ledger/report\n  method: post\n  operationId: ledger_report_dispatch_v1_ledger_report_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/ledger/report/{job_id}\n  method: get\n  operationId: ledger_report_status_v1_ledger_report__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/oracle\n  method: post\n  operationId: oracle_v1_oracle_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parse/datetime\n  method: post\n  operationId: parse_datetime_v1_parse_datetime_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/price/token\n  method: post\n  operationId: token_price_post_v1_price_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/resolve/name\n  method: post\n  operationId: resolve_name_post_v1_resolve_name_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/roast\n  method: post\n  operationId: roast_v1_roast_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/roll\n  method: post\n  operationId: roll_v1_roll_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/screen\n  method: post\n  operationId: screen_post_v1_screen_post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tldr\n  method: post\n  operationId: tldr_v1_tldr_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/agentic-access/anchor-x402-agentic-access.yml
summary_line: 24 operations · 20 acting · 2 human-in-the-loop
tags:
- Company
- x402
- Agents
- Payments
- Blockchain
- MCP
- Web3
- pay-per-call
- Agentic Payments
- Stablecoins
- Compliance
- Attestation
- A2A
---

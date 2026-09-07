---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 22
api_specs:
- filename: hostdefi-token-risk-api-openapi.yml
  format: yaml
  label: HostDeFi Token Risk API
  slug: hostdefi-token-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-token-risk-api-openapi.yml
- filename: hostdefi-analyze-token-api-openapi.yml
  format: yaml
  label: HostDeFi Analyze Token API
  slug: hostdefi-analyze-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-analyze-token-api-openapi.yml
- filename: hostdefi-health-api-openapi.yml
  format: yaml
  label: HostDeFi Health API
  slug: hostdefi-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-health-api-openapi.yml
- filename: hostdefi-keys-api-openapi.yml
  format: yaml
  label: HostDeFi Keys API
  slug: hostdefi-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-keys-api-openapi.yml
- filename: hostdefi-scan-api-openapi.yml
  format: yaml
  label: HostDeFi Scan API
  slug: hostdefi-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-scan-api-openapi.yml
- filename: hostdefi-usage-api-openapi.yml
  format: yaml
  label: HostDeFi Usage API
  slug: hostdefi-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-usage-api-openapi.yml
- filename: hostdefi-x402-machine-payable-api-openapi.yml
  format: yaml
  label: HostDeFi x402 (machine-payable) API
  slug: hostdefi-x402-machine-payable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/openapi/hostdefi-x402-machine-payable-api-openapi.yml
consequence_counts:
  physical: 2
  read: 22
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hostdefi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/keys
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/x402/keys
operation_count: 32
overview: 'HostDeFi exposes 32 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 8 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HostDeFi
provider_slug: hostdefi
slug: hostdefi-agentic-access
source_filename: hostdefi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: generated\nsource: openapi/hostdefi-analyze-token-api-openapi.yml, openapi/hostdefi-health-api-openapi.yml,\n  openapi/hostdefi-keys-api-openapi.yml, openapi/hostdefi-scan-api-openapi.yml, openapi/hostdefi-token-risk-api-openapi.yml,\n  openapi/hostdefi-usage-api-openapi.yml, openapi/hostdefi-x402-machine-payable-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    acting: 10\n    connected: 22\n  by_consequence:\n    write: 8\n    read: 22\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /analyze-token\n  method: post\n  operationId: postAnalyzeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys\n  method: post\n  operationId: postKeys\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scan\n  method: post\n  operationId: postScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/token-risk/{chain}/{address}\n  method: get\n  operationId: getTokenRisk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/token-risk\n  method: post\n  operationId: postTokenRisk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/token-risk/batch\n  method: post\n  operationId: postTokenRiskBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/token-risk/{chain}/{address}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/token-risk/history/{chain}/{address}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/token-risk\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/x402/token-risk/batch\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/pricing\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/signals/solana/{mint}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/authority/solana/{mint}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/portfolio\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/radar\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/keys\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/obituaries\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/listings/{chain}\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/datasets/safety-snapshot\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/radar/history\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/provider-risk\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/provider-risk/all\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/swap/evm/quote\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/swap/evm/price\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/token-risk/deep/{chain}/{address}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/token-risk/report/{chain}/{address}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/wallet\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/launches\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/predict/markets\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/predict/history\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hostdefi/refs/heads/main/agentic-access/hostdefi-agentic-access.yml
summary_line: 32 operations · 10 acting
tags:
- Solana
- Token Risk
- DeFi
- rug pull
- x402
---

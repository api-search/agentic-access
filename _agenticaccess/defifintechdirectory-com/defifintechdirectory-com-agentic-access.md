---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 4
api_specs:
- filename: defifintechdirectory-com-coming-api-openapi.yml
  format: yaml
  label: DeFi Fintech Directory Coming API
  slug: defifintechdirectory-com-coming-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/defifintechdirectory-com/openapi/defifintechdirectory-com-coming-api-openapi.yml
- filename: defifintechdirectory-com-local-api-openapi.yml
  format: yaml
  label: DeFi Fintech Directory Local API
  slug: defifintechdirectory-com-local-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/defifintechdirectory-com/openapi/defifintechdirectory-com-local-api-openapi.yml
- filename: defifintechdirectory-com-local-capability-api-openapi.yml
  format: yaml
  label: DeFi Fintech Directory Local Capability API
  slug: defifintechdirectory-com-local-capability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/defifintechdirectory-com/openapi/defifintechdirectory-com-local-capability-api-openapi.yml
- filename: defifintechdirectory-com-meta-api-openapi.yml
  format: yaml
  label: DeFi Fintech Directory Meta API
  slug: defifintechdirectory-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/defifintechdirectory-com/openapi/defifintechdirectory-com-meta-api-openapi.yml
- filename: defifintechdirectory-com-skill-pack-api-openapi.yml
  format: yaml
  label: DeFi Fintech Directory Skill Pack API
  slug: defifintechdirectory-com-skill-pack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/defifintechdirectory-com/openapi/defifintechdirectory-com-skill-pack-api-openapi.yml
- filename: defifintechdirectory-com-tools-api-openapi.yml
  format: yaml
  label: DeFi Fintech Directory Tools API
  slug: defifintechdirectory-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/defifintechdirectory-com/openapi/defifintechdirectory-com-tools-api-openapi.yml
consequence_counts:
  physical: 2
  read: 4
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Defifintechdirectory Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tools/ship_gate_audit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tools/ship_gate_audit
operation_count: 22
overview: 'DeFi Fintech Directory exposes 22 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 16 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DeFi Fintech Directory
provider_slug: defifintechdirectory-com
slug: defifintechdirectory-com-agentic-access
source_filename: defifintechdirectory-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/defifintechdirectory-com-gateway-openapi.yml, openapi/defifintechdirectory-com-tools-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 18\n    connected: 4\n  by_consequence:\n    write: 16\n    physical: 2\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /tools/game_launch_kit\n  method: post\n  operationId: game_launch_kit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/store_art_prompt_pack\n\
  \  method: post\n  operationId: store_art_prompt_pack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/ship_gate_audit\n  method: post\n  operationId: ship_gate_audit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/text_sha256\n  method: post\n  operationId: text_sha256\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/json_normalize\n  method: post\n  operationId: json_normalize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/json_csv_convert\n  method: post\n  operationId: json_csv_convert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/url_normalize\n  method: post\n  operationId: url_normalize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/cron_next_utc\n  method: post\n  operationId: cron_next_utc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/utm_url_build\n  method: post\n  operationId: utm_url_build\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/base64_text_codec\n  method: post\n  operationId: base64_text_codec\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /packs/designer_pack\n  method: get\n  operationId: designer_pack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packs/marketer_pack\n  method: get\n  operationId: marketer_pack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packs/game_dev_pack\n  method: get\n  operationId: game_dev_pack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/game_launch_kit\n  method: post\n  operationId: gameLaunchKit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/store_art_prompt_pack\n  method: post\n  operationId: storeArtPromptPack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/ship_gate_audit\n  method: post\n  operationId: shipGateAudit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/companion_book_outline\n  method: post\n  operationId: companionBookOutline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/stickman_short_script\n  method: post\n  operationId: stickmanShortScript\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/directory_search\n  method: post\n\
  \  operationId: directorySearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/x402_preflight\n  method: post\n  operationId: x402Preflight\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/listing_health_check\n  method: post\n  operationId: listingHealthCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n"
source_yaml_url: https://artifacts.apis.io/defifintechdirectory-com/agentic-access/defifintechdirectory-com-agentic-access.yml
summary_line: 22 operations · 18 acting
tags:
- Company
- DeFi
- Fintech
- x402
- Micropayments
- USDC
- Base
- AI Agents
- Directory
- MCP
---

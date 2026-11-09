---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 2
api_specs:
- filename: agentic-endpoints-com-compress-api-openapi.yml
  format: yaml
  label: Agentic Endpoints Compress API
  slug: agentic-endpoints-com-compress-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-endpoints-com/openapi/agentic-endpoints-com-compress-api-openapi.yml
- filename: agentic-endpoints-com-credits-api-openapi.yml
  format: yaml
  label: Agentic Endpoints Credits API
  slug: agentic-endpoints-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-endpoints-com/openapi/agentic-endpoints-com-credits-api-openapi.yml
- filename: agentic-endpoints-com-meetings-api-openapi.yml
  format: yaml
  label: Agentic Endpoints Meetings API
  slug: agentic-endpoints-com-meetings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-endpoints-com/openapi/agentic-endpoints-com-meetings-api-openapi.yml
- filename: agentic-endpoints-com-once-key-api-openapi.yml
  format: yaml
  label: Agentic Endpoints Once Key API
  slug: agentic-endpoints-com-once-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-endpoints-com/openapi/agentic-endpoints-com-once-key-api-openapi.yml
- filename: agentic-endpoints-com-pdf-parse-api-openapi.yml
  format: yaml
  label: Agentic Endpoints Pdf Parse API
  slug: agentic-endpoints-com-pdf-parse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-endpoints-com/openapi/agentic-endpoints-com-pdf-parse-api-openapi.yml
- filename: agentic-endpoints-com-reach-api-openapi.yml
  format: yaml
  label: Agentic Endpoints Reach API
  slug: agentic-endpoints-com-reach-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-endpoints-com/openapi/agentic-endpoints-com-reach-api-openapi.yml
- filename: agentic-endpoints-com-scrape-api-openapi.yml
  format: yaml
  label: Agentic Endpoints Scrape API
  slug: agentic-endpoints-com-scrape-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-endpoints-com/openapi/agentic-endpoints-com-scrape-api-openapi.yml
- filename: agentic-endpoints-com-vault-api-openapi.yml
  format: yaml
  label: Agentic Endpoints Vault API
  slug: agentic-endpoints-com-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-endpoints-com/openapi/agentic-endpoints-com-vault-api-openapi.yml
- filename: agentic-endpoints-com-x402-api-openapi.yml
  format: yaml
  label: Agentic Endpoints X402 API
  slug: agentic-endpoints-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-endpoints-com/openapi/agentic-endpoints-com-x402-api-openapi.yml
consequence_counts:
  physical: 4
  read: 2
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentic Endpoints Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /credits/buy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /credits/buy-25
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /reach
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /x402/verify
operation_count: 26
overview: 'Agentic Endpoints exposes 26 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 20 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agentic Endpoints
provider_slug: agentic-endpoints-com
slug: agentic-endpoints-com-agentic-access
source_filename: agentic-endpoints-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/agentic-endpoints-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    acting: 24\n    connected: 2\n  by_consequence:\n    write: 20\n    physical: 4\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /once-key\n  method: post\n  operationId: once_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scrape\n  method: post\n  operationId: scrape\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pdf-parse\n  method: post\n  operationId: pdf_parse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compress\n  method: post\n  operationId: compress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vault/store\n  method: post\n  operationId: vault_store\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vault/delete\n  method: post\n  operationId: vault_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credits/buy\n  method: post\n  operationId: credits_buy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credits/buy-25\n\
  \  method: post\n  operationId: credits_buy_25\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meetings/import\n  method: post\n  operationId: meetings_import\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meetings/search\n  method: post\n  operationId: meetings_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402/verify\n  method: post\n  operationId: x402_verify\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reach\n  method: post\n  operationId: reach\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reach/report\n  method: post\n  operationId: reach_report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meetings/summarize\n  method: post\n  operationId: meetings_summarize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meetings/get\n  method: post\n  operationId: meetings_get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meetings/list\n  method: post\n  operationId: meetings_list\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meetings/delete\n  method: post\n  operationId: meetings_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vault/list\n  method: post\n  operationId: vault_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vault/exists\n  method: post\n  operationId:\
  \ vault_exists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vault/retrieve\n  method: post\n  operationId: vault_retrieve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /once-key/complete\n  method: post\n  operationId: once_key_complete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /vault/rotate-token\n  method: post\n  operationId: vault_rotate_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /once-key/release\n  method: post\n  operationId: once_key_release\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credits/trial\n  method: post\n  operationId: credits_trial\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credits/balance\n  method: get\n  operationId: credits_balance_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credits/balance\n  method: post\n  operationId: credits_balance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agentic-endpoints-com/agentic-access/agentic-endpoints-com-agentic-access.yml
summary_line: 26 operations · 24 acting
tags:
- Artificial Intelligence
- Agents
- Payments
- Micro-utilities
- Base
---

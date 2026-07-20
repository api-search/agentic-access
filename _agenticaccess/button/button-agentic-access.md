---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 4
api_specs:
- filename: button-brands-api-openapi.json
  format: json
  label: Button Brands API
  slug: button-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/openapi/button-brands-api-openapi.json
- filename: button-billing-api-openapi.json
  format: json
  label: Button Billing API
  slug: button-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/openapi/button-billing-api-openapi.json
- filename: button-links-api-openapi.json
  format: json
  label: Button Links API
  slug: button-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/openapi/button-links-api-openapi.json
- filename: button-shortlink-api-openapi.json
  format: json
  label: Button Shortlink API
  slug: button-shortlink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/openapi/button-shortlink-api-openapi.json
- filename: button-offers-api-openapi.json
  format: json
  label: Button Offers API
  slug: button-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/openapi/button-offers-api-openapi.json
consequence_counts:
  read: 4
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Button Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Button exposes 8 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Button
provider_slug: button
slug: button-agentic-access
source_filename: button-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/button-billing-api-openapi.json, openapi/button-brands-api-openapi.json, openapi/button-links-api-openapi.json,\n  openapi/button-offers-api-openapi.json, openapi/button-shortlink-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 4\n    acting: 4\n  by_consequence:\n    read: 4\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts\n  method: get\n  operationId: list-accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/transactions\n  method: get\n  operationId: list-transactions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: get\n  operationId: list-transactions-all\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: list-brand-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: post\n  operationId: generate-a-link\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offers\n  method: post\n  operationId: offers\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /create/\n  method: post\n  operationId: generate-a-brand-shortlink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /create\n  method: post\n  operationId: generate-a-shortlink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/button/refs/heads/main/agentic-access/button-agentic-access.yml
summary_line: 8 operations · 4 acting
tags:
- Commerce
- Affiliate Marketing
- Mobile
- Attribution
- Deep Linking
- Retail Media
- Analytics
- Advertising
- Links
---

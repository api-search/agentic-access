---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 6
api_specs:
- filename: parade-digital-transactions-openapi.yaml
  format: yaml
  label: Parade Transactions API
  slug: parade-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-digital-transactions-openapi.yaml
- filename: parade-load-sync-openapi.yaml
  format: yaml
  label: Parade Load Feed
  slug: parade-load-feed
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-load-sync-openapi.yaml
- filename: parade-partner-webhooks-openapi.yaml
  format: yaml
  label: Parade Syndication Webhooks
  slug: parade-syndication-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-partner-webhooks-openapi.yaml
consequence_counts:
  read: 6
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Parade Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Parade exposes 13 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Parade
provider_slug: parade
slug: parade-agentic-access
source_filename: parade-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/parade-digital-transactions-openapi.yaml, openapi/parade-load-sync-openapi.yaml,\n  openapi/parade-partner-webhooks-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 7\n    connected: 6\n  by_consequence:\n    write: 7\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /ls/syndication/quote\n  method: post\n  operationId: add_quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ls/syndication/quote/{quote_id}\n\
  \  method: get\n  operationId: get_quote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ls/syndication/quote/{quote_id}/cancel\n  method: post\n  operationId: cancel_quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ls/syndication/book\n  method: post\n  operationId: book_now\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ls/syndication/book/{reservation_id}\n  method: get\n  operationId: get_booking\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ls/syndication/loads/{external_posting_id}\n  method: get\n  operationId: get_load\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ls/syndication/post-truck\n  method: post\n  operationId: add_truck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /d/carriers/{dot_number}/onboarding-status\n  method: get\n  operationId: get_carrier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /d/carriers-by-mc/{mc_number}/onboarding-status\n\
  \  method: get\n  operationId: get_carrier_by_mc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ls/syndication/drop\n  method: post\n  operationId: drop_load\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /syndication/loads\n  method: get\n  operationId: search_loads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /your-digital-conversion-notification-webhook\n  method: post\n  operationId: digital_conversion_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /your-carrier-sync-webhook\n  method: post\n  operationId: carrier_sync_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/agentic-access/parade-agentic-access.yml
summary_line: 13 operations · 7 acting
tags:
- Company
- Freight
- Logistics
- Trucking
- Supply Chain
- Capacity Management
- Freight Brokerage
- Transportation
- Load Board
- Artificial Intelligence
---

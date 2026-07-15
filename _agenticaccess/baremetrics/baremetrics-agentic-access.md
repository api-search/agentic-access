---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 12
api_specs:
- filename: llms.txt
  format: yaml
  label: Baremetrics API
  slug: baremetrics-api
  spec_type: OpenAPI
  url: https://developers.baremetrics.com/llms.txt
consequence_counts:
  read: 12
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Baremetrics Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Baremetrics exposes 14 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Baremetrics
provider_slug: baremetrics
slug: baremetrics-agentic-access
source_filename: baremetrics-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/baremetrics-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 12\n    acting: 2\n  by_consequence:\n    read: 12\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/{source_id}/charges\n  method: get\n  operationId: list-charges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{source_id}/charges/{oid}\n  method: get\n  operationId: show-charge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{source_id}/customers\n\
  \  method: get\n  operationId: list-customers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{source_id}/customers/{oid}\n  method: get\n  operationId: show-customer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{source_id}/subscriptions\n  method: get\n  operationId: list-subscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{source_id}/subscriptions/{oid}\n  method: get\n  operationId: show-subscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{source_id}/events\n  method: get\n  operationId: list-events\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metrics/{metric}\n  method: get\n  operationId: show-metric\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{source_id}/plans\n  method: get\n  operationId: list-plans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{source_id}/plans/{oid}\n  method: get\n  operationId: show-plan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/annotations\n  method: get\n  operationId: list-annotations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/annotations\n  method: post\n  operationId: create-annotation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/annotations/{id}\n  method: get\n  operationId: show-annotation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/annotations/{id}\n  method: delete\n  operationId: delete-annotation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baremetrics/refs/heads/main/agentic-access/baremetrics-agentic-access.yml
summary_line: 14 operations · 2 acting
tags:
- Subscription Analytics
- MRR
- ARR
- Churn Rate
- LTV
- Revenue
- Stripe
- Financial Metrics
- SaaS
---

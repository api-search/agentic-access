---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 5
api_specs:
- filename: ship24-tracking-api.yaml
  format: yaml
  label: Ship24 Tracking API
  slug: ship24-tracking-api
  spec_type: OpenAPI
  url: https://docs.ship24.com/assets/openapi/ship24-tracking-api.yaml
consequence_counts:
  physical: 1
  read: 5
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ship24 Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /public/v1/trackers/{trackerId}/webhook-events/resend
operation_count: 11
overview: 'Ship24 exposes 11 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 5 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ship24
provider_slug: ship24
slug: ship24-agentic-access
source_filename: ship24-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ship24-tracking-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 6\n    connected: 5\n  by_consequence:\n    write: 5\n    read: 5\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /public/v1/trackers\n  method: post\n  operationId: create-tracker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/trackers\n  method: get\n  operationId: list-trackers\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/trackers/bulk\n  method: post\n  operationId: bulk-create-trackers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/trackers/track\n  method: post\n  operationId: create-tracker-and-get-tracking-results\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/trackers/{trackerId}\n  method: get\n  operationId: get-tracker-by-trackerId\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/trackers/{trackerId}\n  method: patch\n  operationId: update-tracker-by-trackerId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/trackers/search/{trackingNumber}/results\n  method: get\n  operationId: get-tracking-results-of-trackers-by-tracking-number\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/trackers/{trackerId}/results\n  method: get\n  operationId: get-tracking-results-of-tracker-by-trackerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/couriers\n  method: get\n  operationId: get-couriers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/tracking/search\n  method: post\n  operationId: get-tracking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/trackers/{trackerId}/webhook-events/resend\n  method: post\n  operationId: resend-webhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ship24/refs/heads/main/agentic-access/ship24-agentic-access.yml
summary_line: 11 operations · 6 acting
tags:
- Tracking
- Logistics
- Shipping
- Couriers
- Parcels
- Webhooks
- Ecommerce
- PostPurchase
---

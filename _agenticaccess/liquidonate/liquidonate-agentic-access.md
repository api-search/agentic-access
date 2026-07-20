---
acting_count: 9
action_class_counts:
  acting: 9
api_specs:
- filename: liquidonate-magicmatch-openapi.yml
  format: yaml
  label: MagicMatch by LiquiDonate
  slug: magicmatch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquidonate/refs/heads/main/openapi/liquidonate-magicmatch-openapi.yml
- filename: liquidonate-returnsdirect-openapi.yml
  format: yaml
  label: ReturnsDirect by LiquiDonate (Beta)
  slug: returnsdirect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquidonate/refs/heads/main/openapi/liquidonate-returnsdirect-openapi.yml
consequence_counts:
  physical: 5
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Liquidonate Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/match/ship
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/matchAndShip
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/matchAndShip/estimate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/ship
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /webhooks/external-order
operation_count: 9
overview: 'LiquiDonate exposes 9 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 write and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LiquiDonate
provider_slug: liquidonate
slug: liquidonate-agentic-access
source_filename: liquidonate-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/liquidonate-magicmatch-openapi.yml, openapi/liquidonate-returnsdirect-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 9\n  by_consequence:\n    write: 4\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/setupRetailer\n  method: post\n  operationId: setupRetailer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/getRetailer\n  method: post\n  operationId: getRetailer\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/matchAndShip/estimate\n  method: post\n  operationId: estimateMatchAndShip\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/matchAndShip\n  method: post\n  operationId: matchAndShip\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/match\n  method: post\n  operationId: match\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/match/ship\n  method: post\n  operationId: attachLabelsToMatch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ship\n  method: post\n  operationId: ship\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/donate\n  method: post\n  operationId: donate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/external-order\n  method: post\n  operationId: pushExternalOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquidonate/refs/heads/main/agentic-access/liquidonate-agentic-access.yml
summary_line: 9 operations · 9 acting
tags:
- Reverse Logistics
- Returns Management
- Donations
- Nonprofits
- Retail
- Ecommerce
- Sustainability
- Circular Economy
- Shipping
- Supply Chain
- Excess Inventory
- Company
---

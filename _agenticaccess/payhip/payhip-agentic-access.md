---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 3
api_specs:
- filename: payhip-openapi.yml
  format: yaml
  label: Payhip Coupons API
  slug: payhip-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payhip/refs/heads/main/openapi/payhip-openapi.yml
- filename: payhip-openapi.yml
  format: yaml
  label: Payhip License Keys API
  slug: payhip-license-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payhip/refs/heads/main/openapi/payhip-openapi.yml
- filename: payhip-openapi.yml
  format: yaml
  label: Payhip Webhooks API
  slug: payhip-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payhip/refs/heads/main/openapi/payhip-openapi.yml
consequence_counts:
  read: 3
  safety-critical: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Payhip Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /license/disable
operation_count: 8
overview: 'Payhip exposes 8 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 4 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Payhip
provider_slug: payhip
slug: payhip-agentic-access
source_filename: payhip-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/payhip-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 5\n    connected: 3\n  by_consequence:\n    write: 4\n    read: 3\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /coupons\n  method: post\n  operationId: createCoupon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coupons\n  method: get\n  operationId: listCoupons\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coupons/{id}\n  method: get\n  operationId: getCoupon\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /license/verify\n  method: get\n  operationId: verifyLicense\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /license/enable\n  method: put\n  operationId: enableLicense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /license/disable\n  method: put\n  operationId: disableLicense\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /license/usage\n  method: put\n  operationId: increaseLicenseUsage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /license/decrease\n  method: put\n  operationId: decreaseLicenseUsage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payhip/refs/heads/main/agentic-access/payhip-agentic-access.yml
summary_line: 8 operations · 5 acting · 1 human-in-the-loop
tags:
- E-commerce
- Digital Products
- Memberships
- Creators
- Coupons
- License Keys
- Webhooks
- Payments
---

---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 4
api_specs:
- filename: maya-mobile-openapi.yml
  format: yaml
  label: Maya Mobile Plans and Products API
  slug: plans-products
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-openapi.yml
- filename: maya-mobile-openapi.yml
  format: yaml
  label: Maya Mobile eSIMs and Provisioning API
  slug: esims-provisioning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-openapi.yml
- filename: maya-mobile-openapi.yml
  format: yaml
  label: Maya Mobile Usage and Topup API
  slug: usage-topup
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-openapi.yml
- filename: maya-mobile-openapi.yml
  format: yaml
  label: Maya Mobile Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-openapi.yml
- filename: maya-mobile-openapi.yml
  format: yaml
  label: Maya Mobile Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-openapi.yml
consequence_counts:
  physical: 3
  read: 4
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Maya Mobile Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /esims
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /esims/{esimId}/topup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
operation_count: 9
overview: 'Maya Mobile exposes 9 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 2 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Maya Mobile
provider_slug: maya-mobile
slug: maya-mobile-agentic-access
source_filename: maya-mobile-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/maya-mobile-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 4\n    acting: 5\n  by_consequence:\n    read: 4\n    physical: 3\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /plans\n  method: get\n  operationId: listPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /esims\n  method: post\n  operationId: createEsim\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /esims/{esimId}\n  method: get\n  operationId: getEsim\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /esims/{esimId}/suspend\n  method: post\n  operationId: suspendEsim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /esims/{esimId}/reactivate\n  method: post\n  operationId: reactivateEsim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /esims/{esimId}/usage\n  method: get\n  operationId: getEsimUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /esims/{esimId}/topup\n  method: post\n  operationId: topupEsim\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/agentic-access/maya-mobile-agentic-access.yml
summary_line: 9 operations · 5 acting
tags:
- eSIM
- Connectivity
- Mobile Data
- Roaming
- Telecom
---

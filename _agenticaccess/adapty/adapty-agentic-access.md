---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 3
api_specs:
- filename: adapty-openapi.yml
  format: yaml
  label: Adapty Server-Side Profiles API
  slug: adapty-server-side-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapty/refs/heads/main/openapi/adapty-openapi.yml
- filename: adapty-openapi.yml
  format: yaml
  label: Adapty Server-Side Purchases & Transactions API
  slug: adapty-server-side-purchases-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapty/refs/heads/main/openapi/adapty-openapi.yml
- filename: adapty-openapi.yml
  format: yaml
  label: Adapty Server-Side Access Levels API
  slug: adapty-server-side-access-levels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapty/refs/heads/main/openapi/adapty-openapi.yml
- filename: adapty-openapi.yml
  format: yaml
  label: Adapty Server-Side Paywalls & Products API
  slug: adapty-server-side-paywalls-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapty/refs/heads/main/openapi/adapty-openapi.yml
- filename: adapty-openapi.yml
  format: yaml
  label: Adapty Server-Side Integrations API
  slug: adapty-server-side-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapty/refs/heads/main/openapi/adapty-openapi.yml
consequence_counts:
  physical: 3
  read: 3
  safety-critical: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Adapty Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /purchase/profile/revoke-access-level/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /purchase/profile/grant-access-level/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /purchase/set-transaction/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /purchase/stripe/
operation_count: 12
overview: 'Adapty exposes 12 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 5 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Adapty
provider_slug: adapty
slug: adapty-agentic-access
source_filename: adapty-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/adapty-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 3\n    acting: 9\n  by_consequence:\n    read: 3\n    write: 5\n    physical: 3\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /profile/\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/\n  method: post\n  operationId: createProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/\n  method: patch\n  operationId: updateProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/\n  method: delete\n  operationId: deleteProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /purchase/set-transaction/\n  method: post\n  operationId: setTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /purchase/stripe/\n  method: post\n  operationId: validateStripePurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /purchase/profile/grant-access-level/\n  method: post\n  operationId: grantAccessLevel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /purchase/profile/revoke-access-level/\n  method: post\n  operationId: revokeAccessLevel\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /profile/integration-identifiers/\n  method: post\n  operationId: setIntegrationIdentifiers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paywalls/{developer_id}/\n  method: get\n  operationId: getPaywall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paywalls/{developer_id}/\n  method: patch\n  operationId: updatePaywall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paywalls/\n  method: get\n  operationId: listPaywalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adapty/refs/heads/main/agentic-access/adapty-agentic-access.yml
summary_line: 12 operations · 9 acting · 1 human-in-the-loop
tags:
- Mobile
- Subscriptions
- In-App Purchases
- Paywalls
- Analytics
---

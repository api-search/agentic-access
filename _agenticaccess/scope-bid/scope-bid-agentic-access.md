---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 11
api_specs:
- filename: scope-bid-carrier-feed-api-openapi.yml
  format: yaml
  label: scope-bid Carrier Feed API
  slug: scope-bid-carrier-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-carrier-feed-api-openapi.yml
- filename: scope-bid-deliverables-api-openapi.yml
  format: yaml
  label: scope-bid Deliverables API
  slug: scope-bid-deliverables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-deliverables-api-openapi.yml
- filename: scope-bid-dispatches-api-openapi.yml
  format: yaml
  label: scope-bid Dispatches API
  slug: scope-bid-dispatches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-dispatches-api-openapi.yml
- filename: scope-bid-exports-api-openapi.yml
  format: yaml
  label: scope-bid Exports API
  slug: scope-bid-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-exports-api-openapi.yml
- filename: scope-bid-insights-api-openapi.yml
  format: yaml
  label: scope-bid Insights API
  slug: scope-bid-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-insights-api-openapi.yml
- filename: scope-bid-matters-api-openapi.yml
  format: yaml
  label: scope-bid Matters API
  slug: scope-bid-matters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-matters-api-openapi.yml
- filename: scope-bid-partner-authorizations-api-openapi.yml
  format: yaml
  label: scope-bid Partner Authorizations API
  slug: scope-bid-partner-authorizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-partner-authorizations-api-openapi.yml
- filename: scope-bid-scopes-api-openapi.yml
  format: yaml
  label: scope-bid Scopes API
  slug: scope-bid-scopes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-scopes-api-openapi.yml
- filename: scope-bid-vendors-api-openapi.yml
  format: yaml
  label: scope-bid Vendors API
  slug: scope-bid-vendors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-vendors-api-openapi.yml
- filename: scope-bid-webhooks-api-openapi.yml
  format: yaml
  label: scope-bid Webhooks API
  slug: scope-bid-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 11
  safety-critical: 6
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Scope Bid Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/dispatches
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/dispatches/{dispatch_id}/award
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/partner-authorizations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/scopes/{scope_id}/carrier-feed-token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/webhooks/subscriptions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/webhooks/subscriptions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/webhooks/subscriptions/{id}/test
operation_count: 23
overview: 'scope-bid exposes 23 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 5 write, 1 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: scope-bid
provider_slug: scope-bid
slug: scope-bid-agentic-access
source_filename: scope-bid-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/scope-bid-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 12\n    connected: 11\n  by_consequence:\n    write: 5\n    safety-critical: 6\n    read: 11\n    physical: 1\n  human_in_the_loop_required: 6\noperations:\n- path: /api/v1/matters/sync\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/dispatches\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/dispatches/{dispatch_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/dispatches/{dispatch_id}/award\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/scopes/{scope_id}/audit\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /api/v1/exports/ledes/{scope_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/exports/audit/{scopefile}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/scopes/{scope_id}/carrier-feed-token\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/scopes/{scope_id}/carrier-feed-token\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/scopes/{scope_id}/carrier-feed-token\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/carrier-feed/{token}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vendors/roster\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vendors/roster\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/vendors/roster/{vendor_id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/insights/{kind}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/deliverables\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks/subscriptions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/webhooks/subscriptions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks/subscriptions\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/webhooks/subscriptions/{id}/test\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n  \
  \    exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/partner-authorizations\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/partner-authorizations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/partner-authorizations\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/scope-bid/agentic-access/scope-bid-agentic-access.yml
summary_line: 23 operations · 12 acting · 6 human-in-the-loop
tags:
- Construction
- Bidding
- Software-as-a-Service
- Collaboration
- Analytics
---

---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 5
api_specs:
- filename: adrianhomelab-com-billing-api-openapi.yml
  format: yaml
  label: adrianhomelab-com Billing API
  slug: adrianhomelab-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adrianhomelab-com/openapi/adrianhomelab-com-billing-api-openapi.yml
- filename: adrianhomelab-com-lookups-api-openapi.yml
  format: yaml
  label: adrianhomelab-com Lookups API
  slug: adrianhomelab-com-lookups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adrianhomelab-com/openapi/adrianhomelab-com-lookups-api-openapi.yml
consequence_counts:
  read: 5
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Adrianhomelab Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'adrianhomelab-com exposes 8 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: adrianhomelab-com
provider_slug: adrianhomelab-com
slug: adrianhomelab-com-agentic-access
source_filename: adrianhomelab-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/leadgen-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 3\n    connected: 5\n  by_consequence:\n    write: 3\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/subscribe\n  method: post\n  operationId: subscribe_api_subscribe_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/billing/intent\n  method: get\n  operationId: billing_intent_api_billing_intent_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/billing/company/{cui\n  method: get\n  operationId: billing_company_api_billing_company__cui__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/billing/portal\n  method: post\n  operationId: billing_portal_api_billing_portal_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/billing/portal-link\n  method: post\n  operationId: billing_portal_link_api_billing_portal_link_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fx/eur-ron\n  method: get\n  operationId: fx_eur_ron_api_fx_eur_ron_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup_business\n  method: get\n  operationId: lookup_business_lookup_business_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/adrianhomelab-com/agentic-access/adrianhomelab-com-agentic-access.yml
summary_line: 8 operations · 3 acting
tags:
- Frontend
- React
- JavaScript
- TypeScript
- Web Development
- Portfolio
---

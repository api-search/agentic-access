---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 2
api_specs:
- filename: apollo-insurance-affiliates-api-openapi.yml
  format: yaml
  label: APOLLO Insurance Affiliates API
  slug: apollo-insurance-affiliates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-insurance/refs/heads/main/openapi/apollo-insurance-affiliates-api-openapi.yml
- filename: apollo-insurance-api-api-openapi.yml
  format: yaml
  label: APOLLO Insurance API
  slug: apollo-insurance-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-insurance/refs/heads/main/openapi/apollo-insurance-api-api-openapi.yml
- filename: apollo-insurance-compliance-api-openapi.yml
  format: yaml
  label: APOLLO Insurance Compliance API
  slug: apollo-insurance-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-insurance/refs/heads/main/openapi/apollo-insurance-compliance-api-openapi.yml
- filename: apollo-insurance-quote-api-openapi.yml
  format: yaml
  label: APOLLO Insurance Quote API
  slug: apollo-insurance-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-insurance/refs/heads/main/openapi/apollo-insurance-quote-api-openapi.yml
consequence_counts:
  read: 2
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Apollo Insurance Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'APOLLO Insurance exposes 8 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: APOLLO Insurance
provider_slug: apollo-insurance
slug: apollo-insurance-agentic-access
source_filename: apollo-insurance-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/apollo-insurance-affiliates-legacy.yml, openapi/apollo-insurance-affiliates.yml,\n  openapi/apollo-insurance-covertrack.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 6\n    connected: 2\n  by_consequence:\n    write: 6\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/affiliates/{affiliateId}/tenant/quote\n  method: post\n  operationId: post-api-affiliates-affiliateId-tenant-quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /api/affiliates/{affiliateId}/tenant/application\n  method: post\n  operationId: post-affiliates-affiliateId-application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/affiliates/{affiliateId}/{insuranceType}/application\n  method: post\n  operationId: public-api-affiliates-application-post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/affiliates/{affiliateId}/{insuranceType}/quote\n  method: post\n  operationId: public-api-affiliates-quote-post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compliance/{partnerId}/{propertyId}/{tenantId}\n  method: get\n  operationId: get-compliance-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compliance/{partnerId}/{propertyId}\n  method: get\n  operationId: get-compliance-partnerId-propertyId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quote/tenant/{partnerId}\n  method: post\n  operationId: post-quote-tenant-partnerId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compliance/callback/example\n  method: post\n  operationId: post-compliance-callback-example\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-insurance/refs/heads/main/agentic-access/apollo-insurance-agentic-access.yml
summary_line: 8 operations · 6 acting
tags:
- Insurance
- Canada
- Insurtech
- Brokers
- Embedded Insurance
- Property and Casualty
- Tenant Insurance
- Quoting
- Distribution
- Compliance
---

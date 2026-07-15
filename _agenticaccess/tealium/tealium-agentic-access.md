---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 8
api_specs:
- filename: tealium-collect-http-openapi.yml
  format: yaml
  label: Tealium Collect HTTP API
  slug: tealium-collect-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-collect-http-openapi.yml
- filename: tealium-visitor-profile-openapi.yml
  format: yaml
  label: Tealium Visitor Profile API
  slug: tealium-visitor-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-visitor-profile-openapi.yml
- filename: tealium-visitor-privacy-openapi.yml
  format: yaml
  label: Tealium Visitor Privacy API
  slug: tealium-visitor-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-visitor-privacy-openapi.yml
- filename: tealium-moments-openapi.yml
  format: yaml
  label: Tealium Moments API
  slug: tealium-moments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-moments-openapi.yml
consequence_counts:
  physical: 5
  read: 8
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tealium Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /collect/bulk-event
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /collect/event
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /collect/integration/event/accounts/{account}/profiles/{profile}/datasources/{datasourceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /collect/regional/bulk-event
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /collect/regional/event
operation_count: 15
overview: 'Tealium exposes 15 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 2 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tealium
provider_slug: tealium
slug: tealium-agentic-access
source_filename: tealium-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tealium-authentication-openapi.yml, openapi/tealium-collect-http-openapi.yml,\n  openapi/tealium-moments-openapi.yml, openapi/tealium-visitor-privacy-openapi.yml, openapi/tealium-visitor-profile-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 7\n    connected: 8\n  by_consequence:\n    write: 2\n    read: 8\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/accounts/{account}/profiles/{profile}\n  method: post\n  operationId: generateBearerToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collect/event\n  method: get\n  operationId: collectEventGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collect/event\n  method: post\n  operationId: collectEventPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collect/bulk-event\n  method: post\n  operationId: collectBulkEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collect/regional/event\n  method: post\n  operationId: collectRegionalEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collect/regional/bulk-event\n  method: post\n  operationId: collectRegionalBulkEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collect/integration/event/accounts/{account}/profiles/{profile}/datasources/{datasourceId}\n\
  \  method: post\n  operationId: collectIntegrationEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /personalization/accounts/{account}/profiles/{profile}/engines/{engineId}/visitors/{visitorId}\n  method: get\n  operationId: getMomentsByVisitorId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personalization/accounts/{account}/profiles/{profile}/engines/{engineId}\n  method: get\n  operationId: getMomentsByAttributeValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /privacy/visitor/accounts/{account}/profiles/{profile}\n\
  \  method: get\n  operationId: getPrivacyVisitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /privacy/visitor/accounts/{account}/profiles/{profile}\n  method: delete\n  operationId: deletePrivacyVisitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /privacy/visitor/accounts/{account}/profiles/{profile}/transactions/{transaction_id}\n  method: get\n  operationId: getDeleteTransactionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /privacy/visitor/accounts/{account}/profiles/{profile}/ids\n  method: get\n  operationId: getVisitorIdAttributes\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/visitor/accounts/{account}/profiles/{profile}\n  method: get\n  operationId: getVisitorProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/visitor/historical/accounts/{account}/profiles/{profile}\n  method: get\n  operationId: getHistoricalVisitorProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/agentic-access/tealium-agentic-access.yml
summary_line: 15 operations · 7 acting
tags:
- Customer Data Platform
- CDP
- Tag Management
- AudienceStream
- Real-Time Events
- Visitor Profiles
- Audience Segmentation
- Data Collection
- Privacy Compliance
- Personalization
---

---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 9
api_specs:
- filename: complyadvantage-openapi.yml
  format: yaml
  label: ComplyAdvantage Search API
  slug: complyadvantage-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-openapi.yml
- filename: complyadvantage-openapi.yml
  format: yaml
  label: ComplyAdvantage Monitored Search API
  slug: complyadvantage-monitored-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-openapi.yml
- filename: complyadvantage-openapi.yml
  format: yaml
  label: ComplyAdvantage Case Management API
  slug: complyadvantage-case-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-openapi.yml
- filename: complyadvantage-openapi.yml
  format: yaml
  label: ComplyAdvantage Users API
  slug: complyadvantage-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-openapi.yml
consequence_counts:
  read: 9
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Complyadvantage Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'ComplyAdvantage exposes 19 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ComplyAdvantage
provider_slug: complyadvantage
slug: complyadvantage-agentic-access
source_filename: complyadvantage-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/complyadvantage-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 10\n    connected: 9\n  by_consequence:\n    write: 10\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /searches\n  method: post\n  operationId: createSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /searches\n  method: get\n  operationId: listSearches\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /searches/{id}\n  method: get\n  operationId: getSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /searches/{id}\n  method: patch\n  operationId: updateSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /searches/{id}\n  method: delete\n  operationId: deleteSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /searches/{id}/details\n\
  \  method: get\n  operationId: getSearchDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /searches/{ref}/entities/{entity_provider}\n  method: get\n  operationId: getSearchEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /searches/{id}/certificate\n  method: get\n  operationId: getSearchCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /searches/{id}/entities\n  method: patch\n  operationId: updateSearchEntities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /searches/references\n  method: post\n  operationId: createSearchReferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /searches/{id}/monitors\n  method: get\n  operationId: getMonitoredSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /searches/{id}/monitors\n  method: patch\n  operationId: updateMonitoredSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /searches/{id}/search-profile\n  method: patch\n  operationId: updateSearchProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /searches/{id}/monitor/differences\n  method: get\n  operationId: getMonitoredSearchDifferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /searches/{id}/monitor/acknowledge\n  method: post\n  operationId: acknowledgeMonitoredSearchChanges\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /searches/{id}/comments\n  method: post\n  operationId: createSearchComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /searches/{id}/comments\n  method: get\n  operationId: listSearchComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /searches/{id}/tags/{tag_name}\n  method: delete\n  operationId: detachSearchTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId:\
  \ listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/agentic-access/complyadvantage-agentic-access.yml
summary_line: 19 operations · 10 acting
tags:
- Anti-Money Laundering
- AML
- Fraud Detection
- Sanctions Screening
- Compliance
- PEP Screening
- Adverse Media
- KYC
- Watchlists
- Transaction Monitoring
- Financial Crime
- RegTech
---

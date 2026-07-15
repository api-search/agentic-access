---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 4
api_specs:
- filename: usadf-grants-api-openapi.yml
  format: yaml
  label: USADF Grants Data API
  slug: grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-african-development-foundation/refs/heads/main/openapi/usadf-grants-api-openapi.yml
- filename: usadf-grant-opportunities-api-openapi.yml
  format: yaml
  label: USADF Grant Opportunities API
  slug: grant-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-african-development-foundation/refs/heads/main/openapi/usadf-grant-opportunities-api-openapi.yml
consequence_counts:
  read: 4
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Us African Development Foundation Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'US African Development Foundation exposes 7 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: US African Development Foundation
provider_slug: us-african-development-foundation
slug: us-african-development-foundation-agentic-access
source_filename: us-african-development-foundation-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/usadf-grant-opportunities-api-openapi.yml, openapi/usadf-grants-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 3\n    connected: 4\n  by_consequence:\n    write: 3\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /opportunities/search\n  method: post\n  operationId: searchOpportunities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opportunities/{opportunityId}\n  method: get\n\
  \  operationId: getOpportunity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/search/spending_by_award/\n  method: post\n  operationId: searchAwards\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/awards/{award_id}/\n  method: get\n  operationId: getAward\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/agency/166/awards/\n  method: get\n  operationId: getAgencyAwards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v2/recipient/duns/{uei}/\n  method: get\n  operationId: getRecipient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/search/spending_by_geography/\n  method: post\n  operationId: getSpendingByCountry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-african-development-foundation/refs/heads/main/agentic-access/us-african-development-foundation-agentic-access.yml
summary_line: 7 operations · 3 acting
tags:
- Federal Government
- International Development
- Africa
- Grants
- Nonprofit
- Economic Development
---

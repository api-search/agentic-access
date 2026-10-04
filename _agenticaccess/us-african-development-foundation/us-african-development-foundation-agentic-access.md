---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: us-african-development-foundation-agency-api-openapi.yml
  format: yaml
  label: US African Development Foundation Agency API
  slug: us-african-development-foundation-agency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-african-development-foundation/refs/heads/main/openapi/us-african-development-foundation-agency-api-openapi.yml
- filename: us-african-development-foundation-awards-api-openapi.yml
  format: yaml
  label: US African Development Foundation Awards API
  slug: us-african-development-foundation-awards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-african-development-foundation/refs/heads/main/openapi/us-african-development-foundation-awards-api-openapi.yml
- filename: us-african-development-foundation-opportunities-api-openapi.yml
  format: yaml
  label: US African Development Foundation Opportunities API
  slug: us-african-development-foundation-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-african-development-foundation/refs/heads/main/openapi/us-african-development-foundation-opportunities-api-openapi.yml
- filename: us-african-development-foundation-recipients-api-openapi.yml
  format: yaml
  label: US African Development Foundation Recipients API
  slug: us-african-development-foundation-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-african-development-foundation/refs/heads/main/openapi/us-african-development-foundation-recipients-api-openapi.yml
- filename: us-african-development-foundation-spending-api-openapi.yml
  format: yaml
  label: US African Development Foundation Spending API
  slug: us-african-development-foundation-spending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-african-development-foundation/refs/heads/main/openapi/us-african-development-foundation-spending-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Us African Development Foundation Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'US African Development Foundation exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: US African Development Foundation
provider_slug: us-african-development-foundation
slug: us-african-development-foundation-agentic-access
source_filename: us-african-development-foundation-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/us-african-development-foundation-agency-api-openapi.yml, openapi/us-african-development-foundation-awards-api-openapi.yml,\n  openapi/us-african-development-foundation-opportunities-api-openapi.yml, openapi/us-african-development-foundation-recipients-api-openapi.yml,\n  openapi/us-african-development-foundation-spending-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/agency/166/awards/\n  method: get\n  operationId: getAgencyAwards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v2/search/spending_by_award/\n  method: post\n  operationId: searchAwards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/awards/{award_id}/\n  method: get\n  operationId: getAward\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/search\n  method: post\n  operationId: searchOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{opportunityId}\n  method: get\n  operationId: getOpportunity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/recipient/duns/{uei}/\n  method:\
  \ get\n  operationId: getRecipient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/search/spending_by_geography/\n  method: post\n  operationId: getSpendingByCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-african-development-foundation/refs/heads/main/agentic-access/us-african-development-foundation-agentic-access.yml
summary_line: 7 operations
tags:
- Federal Government
- International Development
- Africa
- Grants
- Non-Profit
- Economic Development
---

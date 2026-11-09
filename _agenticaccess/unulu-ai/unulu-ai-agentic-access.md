---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 3
api_specs:
- filename: unulu-ai-claims-api-openapi.yml
  format: yaml
  label: unulu-ai Claims API
  slug: unulu-ai-claims-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unulu-ai/openapi/unulu-ai-claims-api-openapi.yml
- filename: unulu-ai-feature-votes-api-openapi.yml
  format: yaml
  label: unulu-ai Feature Votes API
  slug: unulu-ai-feature-votes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unulu-ai/openapi/unulu-ai-feature-votes-api-openapi.yml
- filename: unulu-ai-sites-api-openapi.yml
  format: yaml
  label: unulu-ai Sites API
  slug: unulu-ai-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unulu-ai/openapi/unulu-ai-sites-api-openapi.yml
consequence_counts:
  read: 3
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Unulu Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'unulu-ai exposes 9 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: unulu-ai
provider_slug: unulu-ai
slug: unulu-ai-agentic-access
source_filename: unulu-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/unulu-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 6\n    connected: 3\n  by_consequence:\n    write: 6\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/sites\n  method: post\n  operationId: createSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{site_id}\n  method: get\n  operationId: getSiteState\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{site_id}\n  method: patch\n  operationId: updateSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{site_id}\n  method: delete\n  operationId: deleteSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{site_id}/report-abuse\n  method: post\n  operationId: reportAbuse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/feature-votes\n  method: post\n  operationId: submitFeatureVote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{site_id}/request-edit\n  method: post\n  operationId: requestEditAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{site_id}/edit-verify\n  method: get\n  operationId: verifyEditAccess\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/claims/check-handle\n  method: get\n  operationId: checkHandle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/unulu-ai/agentic-access/unulu-ai-agentic-access.yml
summary_line: 9 operations · 6 acting
tags:
- Company
- Artificial Intelligence
- Link in Bio
- MCP
---

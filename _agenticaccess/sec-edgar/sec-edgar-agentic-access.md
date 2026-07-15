---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: sec-edgar-submissions-openapi.yml
  format: yaml
  label: SEC EDGAR Full-Text Search API
  slug: sec-edgar-full-text-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-edgar/refs/heads/main/openapi/sec-edgar-submissions-openapi.yml
- filename: sec-edgar-submissions-openapi.yml
  format: yaml
  label: SEC EDGAR Submissions API
  slug: sec-edgar-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-edgar/refs/heads/main/openapi/sec-edgar-submissions-openapi.yml
- filename: sec-edgar-submissions-openapi.yml
  format: yaml
  label: SEC EDGAR XBRL Company Facts API
  slug: sec-edgar-xbrl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-edgar/refs/heads/main/openapi/sec-edgar-submissions-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sec Edgar Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'sec-edgar exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: sec-edgar
provider_slug: sec-edgar
slug: sec-edgar-agentic-access
source_filename: sec-edgar-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sec-edgar-submissions-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /submissions/CIK{cik}.json\n  method: get\n  operationId: getCompanySubmissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/xbrl/companyfacts/CIK{cik}.json\n  method: get\n  operationId: getCompanyFacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/xbrl/companyconcept/CIK{cik}/{taxonomy}/{concept}.json\n\
  \  method: get\n  operationId: getCompanyConcept\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/xbrl/frames/{taxonomy}/{concept}/{unit}/{period}.json\n  method: get\n  operationId: getXBRLFrames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /LATEST/search-index\n  method: get\n  operationId: fullTextSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sec-edgar/refs/heads/main/agentic-access/sec-edgar-agentic-access.yml
summary_line: 5 operations
tags: []
---

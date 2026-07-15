---
acting_count: 0
action_class_counts:
  connected: 28
api_specs:
- filename: openlaws-openapi.yml
  format: yaml
  label: OpenLaws Legal Data API
  slug: openlaws
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlaws/refs/heads/main/openapi/openlaws-openapi.yml
consequence_counts:
  read: 28
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openlaws Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'OpenLaws exposes 28 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenLaws
provider_slug: openlaws
slug: openlaws-agentic-access
source_filename: openlaws-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openlaws-openapi.json, openapi/openlaws-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 28\n  by_consequence:\n    read: 28\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/jurisdictions\n  method: get\n  operationId: listJurisdictions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/laws/{law_key}/divisions\n  method: get\n  operationId: getRootDivisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/laws/{law_key}/divisions/{path}\n  method: get\n  operationId: getDivsisionsByPath\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/laws/{law_key}/divisions/updates\n  method: get\n  operationId: getDivisionsUpdatedAfter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/laws/{law_key}/divisions/{starting_path}/updates\n  method: get\n  operationId: getDivisionsByPathUpdatedAfter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/laws/search\n  method: get\n  operationId: keywordSearchDivisionWithinJurisdiction\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/laws/{law_key}/search\n  method: get\n  operationId: keywordSearchDivisionWithinLaw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/laws/citations\n  method: get\n  operationId: lookupByBluebookCitation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/laws\n  method: get\n  operationId: getLawsByJurisdiction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/courts\n\
  \  method: get\n  operationId: getCourtsByJurisdiction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/courts/{court_key}\n  method: get\n  operationId: getCourt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/opinions/search\n  method: get\n  operationId: keywordSearchOpinions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/opinions/citations\n  method: get\n  operationId: lookupOpinionByBluebookCitation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/laws\n  method: get\n  operationId: getLaws\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions\n  method: get\n  operationId: listJurisdictions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/laws/{law_key}/divisions\n  method: get\n  operationId: getRootDivisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/laws/{law_key}/divisions/{path}\n  method: get\n  operationId: getDivsisionsByPath\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/laws/{law_key}/divisions/updates\n\
  \  method: get\n  operationId: getDivisionsUpdatedAfter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/laws/{law_key}/divisions/{starting_path}/updates\n  method: get\n  operationId: getDivisionsByPathUpdatedAfter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/laws/search\n  method: get\n  operationId: keywordSearchDivisionWithinJurisdiction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/laws/{law_key}/search\n  method: get\n  operationId: keywordSearchDivisionWithinLaw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/laws/citations\n  method: get\n  operationId: lookupByBluebookCitation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/laws\n  method: get\n  operationId: getLawsByJurisdiction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/courts\n  method: get\n  operationId: getCourtsByJurisdiction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/courts/{court_key}\n  method: get\n  operationId: getCourt\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/opinions/search\n  method: get\n  operationId: keywordSearchOpinions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jurisdictions/{jurisdiction_key}/opinions/citations\n  method: get\n  operationId: lookupOpinionByBluebookCitation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/laws\n  method: get\n  operationId: getLaws\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openlaws/refs/heads/main/agentic-access/openlaws-agentic-access.yml
summary_line: 28 operations
tags:
- Legal
- Law
- Statutes
- Regulations
- Constitutions
- Case Law
- Citations
- Search
- RAG
- LegalTech
- RegTech
- Compliance
- GRC
- Government Data
---

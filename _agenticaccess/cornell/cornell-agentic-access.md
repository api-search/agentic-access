---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: cornell-class-roster-api-openapi.yml
  format: yaml
  label: Cornell Class Roster API
  slug: class-roster
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/openapi/cornell-class-roster-api-openapi.yml
- filename: cornell-library-catalog-api-openapi.yml
  format: yaml
  label: Cornell University Library Catalog Search API
  slug: library-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/openapi/cornell-library-catalog-api-openapi.yml
- filename: cornell-cugir-api-openapi.yml
  format: yaml
  label: Cornell University Cugir API
  slug: cornell-cugir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/openapi/cornell-cugir-api-openapi.yml
consequence_counts:
  read: 11
description: 'Recommended x-agentic-access execution contracts for the surfaces Cornell University itself operates, classified heuristically from the OpenAPI. Regenerated 2026-08-19: the 2026-07-15 file covered 15 operations across five CODI specs, four of which describe surfaces that are dead or vendor-operated (Cornell Dining, Cornell Days, the campus map, and the Localist events calendar). Every operation below is an unauthenticated public read verified live on 2026-08-19.'
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cornell Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Cornell University exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cornell University
provider_slug: cornell
slug: cornell-agentic-access
source_filename: cornell-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: generated\nsource: openapi/cornell-class-roster-api-openapi.yml, openapi/cornell-library-catalog-api-openapi.yml,\n  openapi/cugir-geospatial-api-openapi.yml\ndescription: 'Recommended x-agentic-access execution contracts for the surfaces Cornell University itself\n  operates, classified heuristically from the OpenAPI. Regenerated 2026-08-19: the 2026-07-15 file covered\n  15 operations across five CODI specs, four of which describe surfaces that are dead or vendor-operated\n  (Cornell Dining, Cornell Days, the campus map, and the Localist events calendar). Every operation below\n  is an unauthenticated public read verified live on 2026-08-19.'\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /config/rosters.json\n  method: get\n  source: openapi/cornell-class-roster-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/acadCareers.json\n  method: get\n  source: openapi/cornell-class-roster-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/acadGroups.json\n  method: get\n  source: openapi/cornell-class-roster-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/classLevels.json\n  method: get\n  source: openapi/cornell-class-roster-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/subjects.json\n  method: get\n  source: openapi/cornell-class-roster-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/classes.json\n  method: get\n  source: openapi/cornell-class-roster-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog.json\n  method: get\n  source: openapi/cornell-library-catalog-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/opensearch.xml\n  method: get\n  source: openapi/cornell-library-catalog-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/opensearch.json\n  method: get\n  source: openapi/cornell-library-catalog-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog.json\n  method: get\n  source: openapi/cugir-geospatial-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/{id}.json\n  method: get\n  source: openapi/cugir-geospatial-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/agentic-access/cornell-agentic-access.yml
summary_line: 11 operations
tags:
- University
- Higher Education
- Education
- Ivy League
- United States
- Course Catalog
- Library
- Research Data
- Geospatial
- Identity Federation
---

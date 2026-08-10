---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 3
api_specs:
- filename: eruditus-executive-education-leads-api-openapi.yml
  format: yaml
  label: Eruditus Leads API
  slug: eruditus-executive-education-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eruditus-executive-education/refs/heads/main/openapi/eruditus-executive-education-leads-api-openapi.yml
- filename: eruditus-executive-education-programs-api-openapi.yml
  format: yaml
  label: Eruditus Programs API
  slug: eruditus-executive-education-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eruditus-executive-education/refs/heads/main/openapi/eruditus-executive-education-programs-api-openapi.yml
consequence_counts:
  read: 3
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Eruditus Executive Education Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Eruditus exposes 4 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Eruditus
provider_slug: eruditus-executive-education
slug: eruditus-executive-education-agentic-access
source_filename: eruditus-executive-education-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: generated\nsource: openapi/eruditus-executive-education-leads-openapi.yml, openapi/eruditus-executive-education-programs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 1\n    connected: 3\n  by_consequence:\n    write: 1\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/generic_lead\n  method: post\n  operationId: createGenericLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/programs_api/programs\n\
  \  method: get\n  operationId: listPrograms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/programs_api/schools\n  method: get\n  operationId: listSchools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/programs_api/landing_page_templates\n  method: get\n  operationId: listLandingPageTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eruditus-executive-education/refs/heads/main/agentic-access/eruditus-executive-education-agentic-access.yml
summary_line: 4 operations · 1 acting
tags:
- Company
- Education
- Online Learning
- Executive Education
- EdTech
- Higher Education
- Leads
- Enrollment
- Programs
- Singapore
---

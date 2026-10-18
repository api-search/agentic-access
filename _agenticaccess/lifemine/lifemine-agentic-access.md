---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: lifemine-board-api-openapi.yml
  format: yaml
  label: LifeMine Board API
  slug: lifemine-board-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/openapi/lifemine-board-api-openapi.yml
- filename: lifemine-departments-api-openapi.yml
  format: yaml
  label: LifeMine Departments API
  slug: lifemine-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/openapi/lifemine-departments-api-openapi.yml
- filename: lifemine-education-api-openapi.yml
  format: yaml
  label: LifeMine Education API
  slug: lifemine-education-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/openapi/lifemine-education-api-openapi.yml
- filename: lifemine-jobs-api-openapi.yml
  format: yaml
  label: LifeMine Jobs API
  slug: lifemine-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/openapi/lifemine-jobs-api-openapi.yml
- filename: lifemine-offices-api-openapi.yml
  format: yaml
  label: LifeMine Offices API
  slug: lifemine-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/openapi/lifemine-offices-api-openapi.yml
- filename: lifemine-sections-api-openapi.yml
  format: yaml
  label: LifeMine Sections API
  slug: lifemine-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/openapi/lifemine-sections-api-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lifemine Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'LifeMine exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LifeMine
provider_slug: lifemine
slug: lifemine-agentic-access
source_filename: lifemine-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: generated\nsource: openapi/lifemine-board-api-openapi.yml, openapi/lifemine-departments-api-openapi.yml,\n  openapi/lifemine-education-api-openapi.yml, openapi/lifemine-jobs-api-openapi.yml, openapi/lifemine-offices-api-openapi.yml,\n  openapi/lifemine-sections-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getBoard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /departments\n  method: get\n  operationId: listDepartments\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /departments/{department_id}\n  method: get\n  operationId: getDepartment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /education/degrees\n  method: get\n  operationId: listEducationDegrees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /education/disciplines\n  method: get\n  operationId: listEducationDisciplines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /education/schools\n  method: get\n  operationId: listEducationSchools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{job_id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offices\n  method: get\n  operationId: listOffices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offices/{office_id}\n  method: get\n  operationId: getOffice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections\n  method: get\n  operationId: listSections\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections/{section_id}\n  method: get\n  operationId: getSection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/agentic-access/lifemine-agentic-access.yml
summary_line: 12 operations
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Life Sciences
- Clinical Trials
- Genomics
- Content
- Careers
- WordPress
---

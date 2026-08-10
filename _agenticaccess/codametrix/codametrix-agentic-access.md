---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: codametrix-components-api-openapi.yml
  format: yaml
  label: CodaMetrix Components API
  slug: codametrix-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-components-api-openapi.yml
- filename: codametrix-incidents-api-openapi.yml
  format: yaml
  label: CodaMetrix Incidents API
  slug: codametrix-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-incidents-api-openapi.yml
- filename: codametrix-scheduled-maintenances-api-openapi.yml
  format: yaml
  label: CodaMetrix Scheduled Maintenances API
  slug: codametrix-scheduled-maintenances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-scheduled-maintenances-api-openapi.yml
- filename: codametrix-status-api-openapi.yml
  format: yaml
  label: CodaMetrix Status API
  slug: codametrix-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-status-api-openapi.yml
- filename: codametrix-summary-api-openapi.yml
  format: yaml
  label: CodaMetrix Summary API
  slug: codametrix-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/openapi/codametrix-summary-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Codametrix Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'CodaMetrix exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CodaMetrix
provider_slug: codametrix
slug: codametrix-agentic-access
source_filename: codametrix-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: generated\nsource: openapi/codametrix-status-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /summary.json\n  method: get\n  operationId: getSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status.json\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /components.json\n  method: get\n  operationId: getComponents\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incidents.json\n  method: get\n  operationId: getIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incidents/unresolved.json\n  method: get\n  operationId: getUnresolvedIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scheduled-maintenances.json\n  method: get\n  operationId: getScheduledMaintenances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scheduled-maintenances/upcoming.json\n  method: get\n  operationId: getUpcomingScheduledMaintenances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scheduled-maintenances/active.json\n  method: get\n  operationId: getActiveScheduledMaintenances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codametrix/refs/heads/main/agentic-access/codametrix-agentic-access.yml
summary_line: 8 operations
tags:
- Company
- healthcare
- health-systems
- medical-coding
- autonomous-coding
- revenue-cycle-management
- clinical-documentation
- healthcare-ai
- machine-learning
- natural-language-processing
- ehr-integration
- status
---

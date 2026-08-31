---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: yardi-canada-components-api-openapi.yml
  format: yaml
  label: Yardi Canada Components API
  slug: yardi-canada-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yardi-canada/refs/heads/main/openapi/yardi-canada-components-api-openapi.yml
- filename: yardi-canada-incidents-api-openapi.yml
  format: yaml
  label: Yardi Canada Incidents API
  slug: yardi-canada-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yardi-canada/refs/heads/main/openapi/yardi-canada-incidents-api-openapi.yml
- filename: yardi-canada-maintenance-api-openapi.yml
  format: yaml
  label: Yardi Canada Maintenance API
  slug: yardi-canada-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yardi-canada/refs/heads/main/openapi/yardi-canada-maintenance-api-openapi.yml
- filename: yardi-canada-status-api-openapi.yml
  format: yaml
  label: Yardi Canada Status API
  slug: yardi-canada-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yardi-canada/refs/heads/main/openapi/yardi-canada-status-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Yardi Canada Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Yardi Canada exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Yardi Canada
provider_slug: yardi-canada
slug: yardi-canada-agentic-access
source_filename: yardi-canada-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: generated\nsource: openapi/yardi-canada-status-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /summary.json\n  method: get\n  operationId: getStatusSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status.json\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /components.json\n  method: get\n  operationId: listComponents\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incidents.json\n  method: get\n  operationId: listIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incidents/unresolved.json\n  method: get\n  operationId: listUnresolvedIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scheduled-maintenances.json\n  method: get\n  operationId: listScheduledMaintenances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scheduled-maintenances/upcoming.json\n  method: get\n  operationId: listUpcomingScheduledMaintenances\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scheduled-maintenances/active.json\n  method: get\n  operationId: listActiveScheduledMaintenances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yardi-canada/refs/heads/main/agentic-access/yardi-canada-agentic-access.yml
summary_line: 8 operations
tags:
- Real-Estate
- Canada
- Property Management
- Rentals
- Commercial Real Estate
- PropTech
- Multifamily
- Affordable Housing
- Senior Living
- Investment Management
- Tenancy
- Payments
- MCP
- Artificial Intelligence
---

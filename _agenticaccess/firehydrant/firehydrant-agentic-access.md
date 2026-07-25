---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 17
api_specs:
- filename: firehydrant-audits-api-openapi.yml
  format: yaml
  label: FireHydrant Audits API
  slug: firehydrant-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-audits-api-openapi.yml
- filename: firehydrant-change-events-api-openapi.yml
  format: yaml
  label: FireHydrant Change Events API
  slug: firehydrant-change-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-change-events-api-openapi.yml
- filename: firehydrant-changes-api-openapi.yml
  format: yaml
  label: FireHydrant Changes API
  slug: firehydrant-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-changes-api-openapi.yml
- filename: firehydrant-conversations-api-openapi.yml
  format: yaml
  label: FireHydrant Conversations API
  slug: firehydrant-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-conversations-api-openapi.yml
- filename: firehydrant-environments-api-openapi.yml
  format: yaml
  label: FireHydrant Environments API
  slug: firehydrant-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-environments-api-openapi.yml
- filename: firehydrant-functionalities-api-openapi.yml
  format: yaml
  label: FireHydrant Functionalities API
  slug: firehydrant-functionalities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-functionalities-api-openapi.yml
- filename: firehydrant-incidents-api-openapi.yml
  format: yaml
  label: FireHydrant Incidents API
  slug: firehydrant-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-incidents-api-openapi.yml
- filename: firehydrant-ping-api-openapi.yml
  format: yaml
  label: FireHydrant Ping API
  slug: firehydrant-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-ping-api-openapi.yml
- filename: firehydrant-priorities-api-openapi.yml
  format: yaml
  label: FireHydrant Priorities API
  slug: firehydrant-priorities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-priorities-api-openapi.yml
- filename: firehydrant-runbooks-api-openapi.yml
  format: yaml
  label: FireHydrant Runbooks API
  slug: firehydrant-runbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-runbooks-api-openapi.yml
- filename: firehydrant-scheduled-maintenances-api-openapi.yml
  format: yaml
  label: FireHydrant Scheduled Maintenances API
  slug: firehydrant-scheduled-maintenances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-scheduled-maintenances-api-openapi.yml
- filename: firehydrant-services-api-openapi.yml
  format: yaml
  label: FireHydrant Services API
  slug: firehydrant-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-services-api-openapi.yml
- filename: firehydrant-severities-api-openapi.yml
  format: yaml
  label: FireHydrant Severities API
  slug: firehydrant-severities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-severities-api-openapi.yml
- filename: firehydrant-signals-api-openapi.yml
  format: yaml
  label: FireHydrant Signals API
  slug: firehydrant-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-signals-api-openapi.yml
- filename: firehydrant-teams-api-openapi.yml
  format: yaml
  label: FireHydrant Teams API
  slug: firehydrant-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-teams-api-openapi.yml
consequence_counts:
  read: 17
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Firehydrant Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 38
overview: 'FireHydrant exposes 38 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 21 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FireHydrant
provider_slug: firehydrant
slug: firehydrant-agentic-access
source_filename: firehydrant-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/firehydrant-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    connected: 17\n    acting: 21\n  by_consequence:\n    read: 17\n    write: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /ping\n  method: get\n  operationId: ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incidents\n  method: get\n  operationId: listIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incidents\n  method: post\n  operationId: createIncident\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /incidents/{incident_id}\n  method: get\n  operationId: getIncident\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incidents/{incident_id}\n  method: patch\n  operationId: updateIncident\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /incidents/{incident_id}\n  method: delete\n  operationId: archiveIncident\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /incidents/{incident_id}/close\n  method: put\n  operationId: closeIncident\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /incidents/{incident_id}/notes\n  method: post\n  operationId: createIncidentNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /incidents/{incident_id}/events\n  method: get\n\
  \  operationId: listIncidentEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services\n  method: get\n  operationId: listServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services\n  method: post\n  operationId: createService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/{service_id}\n  method: get\n  operationId: getService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/{service_id}\n  method: patch\n\
  \  operationId: updateService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/{service_id}\n  method: delete\n  operationId: deleteService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments\n  method: get\n  operationId: listEnvironments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments\n  method: post\n  operationId: createEnvironment\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environment_id}\n  method: get\n  operationId: getEnvironment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /functionalities\n  method: get\n  operationId: listFunctionalities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /functionalities\n  method: post\n  operationId: createFunctionality\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams\n  method: post\n  operationId: createTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/{team_id}\n  method: get\n  operationId: getTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runbooks\n  method: get\n  operationId: listRunbooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /runbooks\n  method: post\n  operationId: createRunbook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runbooks/executions\n  method: post\n  operationId: createRunbookExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /changes\n  method: get\n  operationId: listChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changes\n  method: post\n  operationId: createChange\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /change_events\n  method: post\n  operationId: createChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /change_events/{change_event_id}\n  method: get\n  operationId: getChangeEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /change_events/{change_event_id}\n  method: delete\n  operationId: deleteChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversation_id}/comments\n  method: post\n  operationId: createComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signals/events\n  method: post\n  operationId: createSignalsEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /severities\n  method: get\n  operationId: listSeverities\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /severities\n  method: post\n  operationId: createSeverity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /priorities\n  method: get\n  operationId: listPriorities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /priorities\n  method: post\n  operationId: createPriority\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /scheduled_maintenances\n  method: post\n  operationId: createScheduledMaintenance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audits/{audit_event_id}\n  method: get\n  operationId: getAuditEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/agentic-access/firehydrant-agentic-access.yml
summary_line: 38 operations · 21 acting
tags:
- AIOps
- Incident Management
---

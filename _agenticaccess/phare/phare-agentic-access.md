---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 22
api_specs:
- filename: phare-alert-rules-api-openapi.yml
  format: yaml
  label: Phare Alert Rules API
  slug: phare-alert-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-alert-rules-api-openapi.yml
- filename: phare-incidents-api-openapi.yml
  format: yaml
  label: Phare Incidents API
  slug: phare-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-incidents-api-openapi.yml
- filename: phare-integrations-api-openapi.yml
  format: yaml
  label: Phare Integrations API
  slug: phare-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-integrations-api-openapi.yml
- filename: phare-maintenance-windows-api-openapi.yml
  format: yaml
  label: Phare Maintenance Windows API
  slug: phare-maintenance-windows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-maintenance-windows-api-openapi.yml
- filename: phare-monitors-api-openapi.yml
  format: yaml
  label: Phare Monitors API
  slug: phare-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-monitors-api-openapi.yml
- filename: phare-platform-api-openapi.yml
  format: yaml
  label: Phare Platform API
  slug: phare-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-platform-api-openapi.yml
- filename: phare-projects-api-openapi.yml
  format: yaml
  label: Phare Projects API
  slug: phare-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-projects-api-openapi.yml
- filename: phare-reports-api-openapi.yml
  format: yaml
  label: Phare Reports API
  slug: phare-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-reports-api-openapi.yml
- filename: phare-status-pages-api-openapi.yml
  format: yaml
  label: Phare Status Pages API
  slug: phare-status-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-status-pages-api-openapi.yml
- filename: phare-users-api-openapi.yml
  format: yaml
  label: Phare Users API
  slug: phare-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-users-api-openapi.yml
consequence_counts:
  read: 22
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Phare Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 48
overview: 'Phare exposes 48 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 26 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Phare
provider_slug: phare
slug: phare-agentic-access
source_filename: phare-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: generated\nsource: openapi/phare-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 48\n  by_action_class:\n    connected: 22\n    acting: 26\n  by_consequence:\n    read: 22\n    write: 26\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alert-rules\n  method: get\n  operationId: getAlertRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alert-rules\n  method: post\n  operationId: createUptimeAlertRule\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alert-rules/{alertRuleId}\n  method: get\n  operationId: getAlertRule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alert-rules/{alertRuleId}\n  method: post\n  operationId: updateUptimeAlertRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alert-rules/{alertRuleId}\n  method: delete\n  operationId: deleteUptimeAlertRule\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app}/integrations\n  method: get\n  operationId: getIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app}/integrations/{integrationId}\n  method: get\n  operationId: getIntegration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: get\n  operationId: getProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}\n  method: post\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}\n  method: delete\n  operationId: deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uptime/incidents\n  method: get\n  operationId: getUptimeIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uptime/incidents\n  method: post\n  operationId: createUptimeIncident\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uptime/incidents/{incidentId}\n  method: get\n  operationId: getUptimeIncident\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uptime/incidents/{incidentId}\n  method: post\n  operationId: updateUptimeIncident\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uptime/incidents/{incidentId}\n  method: delete\n  operationId: deleteUptimeIncident\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uptime/incidents/{incidentId}/recover\n  method: post\n  operationId: recoverUptimeIncident\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uptime/incidents/{incidentId}/updates\n  method: get\n  operationId: getUptimeIncidentUpdates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uptime/incidents/{incidentId}/updates\n  method: post\n  operationId: createUptimeIncidentUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uptime/incidents/{incidentId}/updates/{incidentUpdateId}\n  method: get\n  operationId: getUptimeIncidentUpdate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uptime/incidents/{incidentId}/updates/{incidentUpdateId}\n  method: post\n  operationId: updateUptimeIncidentUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uptime/incidents/{incidentId}/updates/{incidentUpdateId}\n  method: delete\n  operationId: deleteUptimeIncidentUpdate\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uptime/maintenance-windows\n  method: get\n  operationId: getUptimeMaintenanceWindows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uptime/maintenance-windows\n  method: post\n  operationId: createUptimeMaintenanceWindow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uptime/maintenance-windows/{maintenanceWindowId}\n  method: get\n  operationId: getUptimeMaintenanceWindow\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uptime/maintenance-windows/{maintenanceWindowId}\n  method: post\n  operationId: updateUptimeMaintenanceWindow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uptime/maintenance-windows/{maintenanceWindowId}\n  method: delete\n  operationId: deleteUptimeMaintenanceWindow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uptime/maintenance-windows/{maintenanceWindowId}/cancel\n  method: post\n\
  \  operationId: cancelUptimeMaintenanceWindow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uptime/maintenance-windows/{maintenanceWindowId}/complete\n  method: post\n  operationId: completeUptimeMaintenanceWindow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uptime/monitors\n  method: get\n  operationId: getUptimeMonitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uptime/monitors\n  method: post\n  operationId:\
  \ createUptimeMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uptime/monitors/{monitorId}\n  method: get\n  operationId: getUptimeMonitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uptime/monitors/{monitorId}\n  method: post\n  operationId: updateUptimeMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uptime/monitors/{monitorId}\n  method: delete\n  operationId: deleteUptimeMonitor\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uptime/monitors/{monitorId}/pause\n  method: post\n  operationId: pauseUptimeMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uptime/monitors/{monitorId}/resume\n  method: post\n  operationId: resumeUptimeMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /uptime/monitors/{monitorId}/report\n  method: get\n  operationId: getUptimeMonitorReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uptime/reports\n  method: get\n  operationId: getUptimeReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uptime/status-pages\n  method: get\n  operationId: getUptimeStatusPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uptime/status-pages\n  method: post\n  operationId: createUptimeStatusPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /uptime/status-pages/{statusPageId}\n  method: get\n  operationId: getUptimeStatusPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uptime/status-pages/{statusPageId}\n  method: post\n  operationId: updateUptimeStatusPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uptime/status-pages/{statusPageId}\n  method: delete\n  operationId: deleteUptimeStatusPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /uptime/status-pages/{statusPageId}/current-status\n  method: get\n  operationId: getUptimeStatusPageCurrentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/agentic-access/phare-agentic-access.yml
summary_line: 48 operations · 26 acting
tags:
- Company
- Monitoring
- Incident Management
- Analytics
- European
---

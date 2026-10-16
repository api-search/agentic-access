---
acting_count: 34
action_class_counts:
  acting: 34
  connected: 30
api_specs:
- filename: uptimerobot-alert-contacts-api-openapi.yml
  format: yaml
  label: UptimeRobot Alert Contacts API
  slug: uptimerobot-alert-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-alert-contacts-api-openapi.yml
- filename: uptimerobot-incidents-api-openapi.yml
  format: yaml
  label: UptimeRobot Incidents API
  slug: uptimerobot-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-incidents-api-openapi.yml
- filename: uptimerobot-integrations-api-openapi.yml
  format: yaml
  label: UptimeRobot Integrations API
  slug: uptimerobot-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-integrations-api-openapi.yml
- filename: uptimerobot-maintenance-windows-api-openapi.yml
  format: yaml
  label: UptimeRobot Maintenance Windows API
  slug: uptimerobot-maintenance-windows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-maintenance-windows-api-openapi.yml
- filename: uptimerobot-monitor-groups-api-openapi.yml
  format: yaml
  label: UptimeRobot Monitor Groups API
  slug: uptimerobot-monitor-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-monitor-groups-api-openapi.yml
- filename: uptimerobot-monitors-api-openapi.yml
  format: yaml
  label: UptimeRobot Monitors API
  slug: uptimerobot-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-monitors-api-openapi.yml
- filename: uptimerobot-monitors-bulk-operations-api-openapi.yml
  format: yaml
  label: UptimeRobot Monitors - Bulk Operations API
  slug: uptimerobot-monitors-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-monitors-bulk-operations-api-openapi.yml
- filename: uptimerobot-psp-announcements-api-openapi.yml
  format: yaml
  label: UptimeRobot PSP Announcements API
  slug: uptimerobot-psp-announcements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-psp-announcements-api-openapi.yml
- filename: uptimerobot-public-status-pages-api-openapi.yml
  format: yaml
  label: UptimeRobot Public Status Pages API
  slug: uptimerobot-public-status-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-public-status-pages-api-openapi.yml
- filename: uptimerobot-storm-protection-api-openapi.yml
  format: yaml
  label: UptimeRobot Storm Protection API
  slug: uptimerobot-storm-protection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-storm-protection-api-openapi.yml
- filename: uptimerobot-tags-api-openapi.yml
  format: yaml
  label: UptimeRobot Tags API
  slug: uptimerobot-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-tags-api-openapi.yml
- filename: uptimerobot-user-api-openapi.yml
  format: yaml
  label: UptimeRobot User API
  slug: uptimerobot-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/openapi/uptimerobot-user-api-openapi.yml
consequence_counts:
  read: 30
  safety-critical: 34
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 34
kind: agentic-access
layout: agentic-access
method: generated
name: Uptimerobot Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /alert-contacts
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /alert-contacts/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /alert-contacts/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /incidents/{id}/comments
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /incidents/{id}/comments/{commentId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /incidents/{id}/comments/{commentId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /integrations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /integrations/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /integrations/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /maintenance-windows
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /maintenance-windows/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /maintenance-windows/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /monitor-groups
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /monitor-groups/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /monitor-groups/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /monitors
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /monitors/bulk/pause
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /monitors/bulk/start
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /monitors/bulk/update
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /monitors/storm-protection
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /monitors/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /monitors/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /monitors/{id}/pause
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /monitors/{id}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /monitors/{id}/start
operation_count: 64
overview: 'UptimeRobot exposes 64 API operations that an AI agent could call, of which 34 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read and 34 safety-critical.


  34 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: UptimeRobot
provider_slug: uptimerobot
slug: uptimerobot-agentic-access
source_filename: uptimerobot-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/uptimerobot-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 64\n  by_action_class:\n    acting: 34\n    connected: 30\n  by_consequence:\n    safety-critical: 34\n    read: 30\n  human_in_the_loop_required: 34\noperations:\n- path: /monitors/bulk/pause\n  method: post\n  operationId: BulkMonitorsController_bulkPause\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /monitors/bulk/start\n  method: post\n\
  \  operationId: BulkMonitorsController_bulkStart\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /monitors/bulk/update\n  method: post\n  operationId: BulkMonitorsController_bulkUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /incidents\n  method: get\n  operationId: IncidentsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /incidents/{id}\n  method: get\n  operationId: IncidentsController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incidents/{id}/comments\n  method: get\n  operationId: IncidentsController_listComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incidents/{id}/comments\n  method: post\n  operationId: IncidentsController_createComment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /incidents/{id}/activity-log\n  method: get\n  operationId: IncidentsController_getActivityLog\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incidents/{id}/alerts\n  method: get\n  operationId: IncidentsController_getAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incidents/{id}/comments/{commentId}\n  method: patch\n  operationId: IncidentsController_updateComment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /incidents/{id}/comments/{commentId}\n  method: delete\n  operationId: IncidentsController_deleteComment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /monitor-groups\n  method: post\n  operationId: MonitorGroupsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /monitor-groups\n  method: get\n  operationId: MonitorGroupsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitor-groups/{id}\n  method: get\n  operationId: MonitorGroupsController_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitor-groups/{id}\n  method: patch\n  operationId: MonitorGroupsController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /monitor-groups/{id}\n  method: delete\n  operationId: MonitorGroupsController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /monitors/storm-protection\n  method: get\n  operationId: StormProtectionController_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/storm-protection\n  method: patch\n  operationId: StormProtectionController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /monitors\n  method: get\n  operationId: MonitorsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors\n  method: post\n  operationId: MonitorsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n    \
  \  exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /monitors/uptime-stats\n  method: get\n  operationId: MonitorsController_getUptimeStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/{id}/stats/uptime\n  method: get\n  operationId: MonitorsController_getMonitorUptimeStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/{id}/stats/response-time/all\n  method: get\n  operationId: MonitorsController_getMonitorResponseTimeStatsByRegion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/{id}/stats/response-time\n  method: get\n  operationId:\
  \ MonitorsController_getMonitorResponseTimeStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/{id}/dependency/status\n  method: get\n  operationId: MonitorsController_getDependencyStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/{id}/dependency/incidents\n  method: get\n  operationId: MonitorsController_getDependencyIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/{id}\n  method: get\n  operationId: MonitorsController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/{id}\n  method: patch\n  operationId: MonitorsController_update\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /monitors/{id}\n  method: delete\n  operationId: MonitorsController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /monitors/{id}/reset\n  method: post\n  operationId: MonitorsController_reset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /monitors/{id}/pause\n  method: post\n  operationId: MonitorsController_pause\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /monitors/{id}/start\n  method: post\n  operationId: MonitorsController_start\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /psps\n  method: get\n  operationId: PspController_list\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psps\n  method: post\n  operationId: PspController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /psps/{id}\n  method: get\n  operationId: PspController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psps/{id}\n  method: patch\n  operationId: PspController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /psps/{id}\n  method: delete\n  operationId: PspController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /psps/{pspId}/announcements\n  method: get\n  operationId: PspAnnouncementsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psps/{pspId}/announcements\n  method: post\n  operationId: PspAnnouncementsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /psps/{pspId}/announcements/{id}\n  method: get\n  operationId: PspAnnouncementsController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psps/{pspId}/announcements/{id}\n  method: patch\n  operationId: PspAnnouncementsController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /psps/{pspId}/announcements/{id}\n  method: delete\n  operationId: PspAnnouncementsController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /psps/{pspId}/announcements/{id}/pin\n  method: post\n  operationId: PspAnnouncementsController_pin\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /psps/{pspId}/announcements/{id}/unpin\n  method: post\n  operationId: PspAnnouncementsController_unpin\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n   \
  \   proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /maintenance-windows\n  method: get\n  operationId: MaintenanceWindowsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /maintenance-windows\n  method: post\n  operationId: MaintenanceWindowsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /maintenance-windows/{id}\n  method: get\n  operationId: MaintenanceWindowsController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /maintenance-windows/{id}\n  method: patch\n  operationId: MaintenanceWindowsController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /maintenance-windows/{id}\n  method: delete\n  operationId: MaintenanceWindowsController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/me\n  method: get\n  operationId: UserController_getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/alert-contacts\n  method: get\n  operationId: UserController_getAlertContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/all-alert-contacts\n  method: get\n  operationId: UserController_getAllAlertContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations\n  method: get\n  operationId: IntegrationsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations\n  method: post\n  operationId: IntegrationsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /integrations/{id}\n  method: get\n  operationId: IntegrationsController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations/{id}\n  method: patch\n  operationId: IntegrationsController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /integrations/{id}\n  method: delete\n  operationId: IntegrationsController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /alert-contacts\n  method: get\n  operationId: AlertContactsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alert-contacts\n  method: post\n  operationId: AlertContactsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /alert-contacts/{id}\n  method: get\n  operationId: AlertContactsController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alert-contacts/{id}\n  method: patch\n  operationId: AlertContactsController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /alert-contacts/{id}\n  method: delete\n  operationId: AlertContactsController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /tags\n  method: get\n  operationId: TagsController_getTags\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/{id}\n  method: delete\n  operationId: TagsController_deleteTag\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uptimerobot/refs/heads/main/agentic-access/uptimerobot-agentic-access.yml
summary_line: 64 operations · 34 acting · 34 human-in-the-loop
tags:
- Uptime Monitoring
- Status Pages
- Incident Management
- API
- DevOps
- Monitoring Integrations
---

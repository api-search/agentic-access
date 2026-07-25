---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 22
api_specs:
- filename: checkly-accounts-api-openapi.yml
  format: yaml
  label: Checkly Accounts API
  slug: checkly-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-accounts-api-openapi.yml
- filename: checkly-alert-channels-api-openapi.yml
  format: yaml
  label: Checkly Alert Channels API
  slug: checkly-alert-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-alert-channels-api-openapi.yml
- filename: checkly-analytics-api-openapi.yml
  format: yaml
  label: Checkly Analytics API
  slug: checkly-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-analytics-api-openapi.yml
- filename: checkly-check-alerts-api-openapi.yml
  format: yaml
  label: Checkly Check Alerts API
  slug: checkly-check-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-check-alerts-api-openapi.yml
- filename: checkly-check-groups-api-openapi.yml
  format: yaml
  label: Checkly Check Groups API
  slug: checkly-check-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-check-groups-api-openapi.yml
- filename: checkly-check-results-api-openapi.yml
  format: yaml
  label: Checkly Check Results API
  slug: checkly-check-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-check-results-api-openapi.yml
- filename: checkly-check-statuses-api-openapi.yml
  format: yaml
  label: Checkly Check Statuses API
  slug: checkly-check-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-check-statuses-api-openapi.yml
- filename: checkly-checks-api-openapi.yml
  format: yaml
  label: Checkly Checks API
  slug: checkly-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-checks-api-openapi.yml
- filename: checkly-dashboards-api-openapi.yml
  format: yaml
  label: Checkly Dashboards API
  slug: checkly-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-dashboards-api-openapi.yml
- filename: checkly-heartbeats-api-openapi.yml
  format: yaml
  label: Checkly Heartbeats API
  slug: checkly-heartbeats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-heartbeats-api-openapi.yml
- filename: checkly-incidents-api-openapi.yml
  format: yaml
  label: Checkly Incidents API
  slug: checkly-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-incidents-api-openapi.yml
- filename: checkly-locations-api-openapi.yml
  format: yaml
  label: Checkly Locations API
  slug: checkly-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-locations-api-openapi.yml
- filename: checkly-maintenance-windows-api-openapi.yml
  format: yaml
  label: Checkly Maintenance Windows API
  slug: checkly-maintenance-windows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-maintenance-windows-api-openapi.yml
- filename: checkly-private-locations-api-openapi.yml
  format: yaml
  label: Checkly Private Locations API
  slug: checkly-private-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-private-locations-api-openapi.yml
- filename: checkly-reports-api-openapi.yml
  format: yaml
  label: Checkly Reports API
  slug: checkly-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-reports-api-openapi.yml
- filename: checkly-variables-api-openapi.yml
  format: yaml
  label: Checkly Variables API
  slug: checkly-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-variables-api-openapi.yml
consequence_counts:
  read: 22
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Checkly Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Checkly exposes 27 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Checkly
provider_slug: checkly
slug: checkly-agentic-access
source_filename: checkly-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/checkly-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 22\n    acting: 5\n  by_consequence:\n    read: 22\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{accountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/api-checks/{id}\n\
  \  method: get\n  operationId: getApiCheckAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/browser-checks/{id}\n  method: get\n  operationId: getBrowserCheckAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/metrics/{checkType}\n  method: get\n  operationId: listAnalyticsMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/check-alerts\n  method: get\n  operationId: listCheckAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/check-alerts/{checkId}\n  method: get\n  operationId: getCheckAlerts\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/check-groups\n  method: get\n  operationId: listCheckGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/check-groups\n  method: post\n  operationId: createCheckGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/check-results/{checkId}\n  method: get\n  operationId: listCheckResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/check-results/{checkId}/{checkResultId}\n  method: get\n  operationId:\
  \ getCheckResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/check-statuses\n  method: get\n  operationId: listCheckStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/checks\n  method: get\n  operationId: listChecks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alert-channels\n  method: get\n  operationId: listAlertChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alert-channels\n  method: post\n  operationId: createAlertChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alert-channels/{id}\n  method: get\n  operationId: getAlertChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dashboards\n  method: get\n  operationId: listDashboards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/heartbeats\n  method: get\n  operationId: listHeartbeats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/heartbeats\n  method: post\n  operationId: createHeartbeat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/incidents\n  method: get\n  operationId: listIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/locations\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/maintenance-windows\n  method: get\n  operationId: listMaintenanceWindows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/maintenance-windows\n  method: post\n  operationId: createMaintenanceWindow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/private-locations\n  method: get\n  operationId: listPrivateLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/private-locations\n  method: post\n  operationId: createPrivateLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reports\n  method: get\n  operationId: listReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/variables\n  method: get\n  operationId: listVariables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/agentic-access/checkly-agentic-access.yml
summary_line: 27 operations · 5 acting
tags:
- Monitoring
- Testing
---

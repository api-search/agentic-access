---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 5
api_specs:
- filename: google-cloud-operations-suite-entries-list-api-openapi.yml
  format: yaml
  label: Google Cloud Operations Suite Entries:list API
  slug: google-cloud-operations-suite-entries-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-operations-suite/refs/heads/main/openapi/google-cloud-operations-suite-entries-list-api-openapi.yml
- filename: google-cloud-operations-suite-entries-write-api-openapi.yml
  format: yaml
  label: Google Cloud Operations Suite Entries:write API
  slug: google-cloud-operations-suite-entries-write-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-operations-suite/refs/heads/main/openapi/google-cloud-operations-suite-entries-write-api-openapi.yml
- filename: google-cloud-operations-suite-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Operations Suite Projects API
  slug: google-cloud-operations-suite-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-operations-suite/refs/heads/main/openapi/google-cloud-operations-suite-projects-api-openapi.yml
consequence_counts:
  read: 5
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Operations Suite Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Google Cloud Observability exposes 9 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Observability
provider_slug: google-cloud-operations-suite
slug: google-cloud-operations-suite-agentic-access
source_filename: google-cloud-operations-suite-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/google-cloud-operations-suite-entries-list-api-openapi.yml, openapi/google-cloud-operations-suite-entries-write-api-openapi.yml,\n  openapi/google-cloud-operations-suite-projects-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 5\n    acting: 4\n  by_consequence:\n    read: 5\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/entries:list\n  method: post\n  operationId: listLogEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/entries:write\n  method: post\n  operationId: writeLogEntries\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/projects/{projectId}/timeSeries\n  method: get\n  operationId: listTimeSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/projects/{projectId}/timeSeries\n  method: post\n  operationId: createTimeSeries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/projects/{projectId}/alertPolicies\n  method: get\n  operationId: listAlertPolicies\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/projects/{projectId}/alertPolicies\n  method: post\n  operationId: createAlertPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/dashboards\n  method: get\n  operationId: listDashboards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/dashboards\n  method: post\n  operationId: createDashboard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/projects/{projectId}/uptimeCheckConfigs\n  method: get\n  operationId: listUptimeCheckConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-operations-suite/refs/heads/main/agentic-access/google-cloud-operations-suite-agentic-access.yml
summary_line: 9 operations · 4 acting
tags:
- Error Reporting
- Google Cloud
- Logging
- Monitoring
- Observability
- Profiling
- Stackdriver
- Tracing
---

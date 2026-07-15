---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 10
api_specs:
- filename: openstatus-openapi.yml
  format: yaml
  label: OpenStatus Monitors
  slug: monitors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstatus/refs/heads/main/openapi/openstatus-openapi.yml
- filename: openstatus-openapi.yml
  format: yaml
  label: OpenStatus Incidents
  slug: incidents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstatus/refs/heads/main/openapi/openstatus-openapi.yml
- filename: openstatus-openapi.yml
  format: yaml
  label: OpenStatus Status Reports
  slug: status-reports
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstatus/refs/heads/main/openapi/openstatus-openapi.yml
- filename: openstatus-openapi.yml
  format: yaml
  label: OpenStatus Status Pages
  slug: status-pages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstatus/refs/heads/main/openapi/openstatus-openapi.yml
- filename: openstatus-openapi.yml
  format: yaml
  label: OpenStatus Checks
  slug: checks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstatus/refs/heads/main/openapi/openstatus-openapi.yml
consequence_counts:
  read: 10
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openstatus Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'OpenStatus exposes 22 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenStatus
provider_slug: openstatus
slug: openstatus-agentic-access
source_filename: openstatus-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openstatus-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 10\n    acting: 12\n  by_consequence:\n    read: 10\n    write: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /monitor\n  method: get\n  operationId: getAllMonitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitor\n  method: post\n  operationId: createMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitor/{id}\n  method: get\n  operationId: getMonitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitor/{id}\n  method: put\n  operationId: updateMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitor/{id}\n  method: delete\n  operationId: deleteMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitor/{id}/summary\n\
  \  method: get\n  operationId: getMonitorSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitor/{id}/run\n  method: post\n  operationId: runMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /incident\n  method: get\n  operationId: getAllIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incident/{id}\n  method: get\n  operationId: getIncident\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incident/{id}\n  method:\
  \ put\n  operationId: updateIncident\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status_report\n  method: get\n  operationId: getAllStatusReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status_report\n  method: post\n  operationId: createStatusReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status_report/{id}\n  method: get\n  operationId: getStatusReport\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status_report/{id}\n  method: delete\n  operationId: deleteStatusReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status_report_update\n  method: post\n  operationId: createStatusReportUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /page\n  method: get\n  operationId: getAllPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /page\n  method: post\n  operationId: createPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /page/{id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /page/{id}\n  method: put\n  operationId: updatePage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /page_subscriber\n  method: post\n  operationId: createPageSubscriber\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check\n  method: post\n  operationId: createCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /whoami\n  method: get\n  operationId: getWhoami\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openstatus/refs/heads/main/agentic-access/openstatus-agentic-access.yml
summary_line: 22 operations · 12 acting
tags:
- Monitoring
- Synthetic Monitoring
- Uptime
- Status Pages
- Incidents
- Open Source
- Observability
---

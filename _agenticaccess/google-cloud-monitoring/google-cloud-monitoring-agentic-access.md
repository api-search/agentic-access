---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 7
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google Cloud Monitoring API
  slug: google-cloud-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-monitoring/refs/heads/main/openapi/openapi.yml
consequence_counts:
  read: 7
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Monitoring Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Google Cloud Monitoring exposes 14 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Monitoring
provider_slug: google-cloud-monitoring
slug: google-cloud-monitoring-agentic-access
source_filename: google-cloud-monitoring-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 7\n    acting: 7\n  by_consequence:\n    read: 7\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/projects/{projectId}/timeSeries\n  method: get\n  operationId: listTimeSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/projects/{projectId}/timeSeries\n  method: post\n  operationId: createTimeSeries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/projects/{projectId}/alertPolicies\n  method: get\n  operationId: listAlertPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/projects/{projectId}/alertPolicies\n  method: post\n  operationId: createAlertPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/projects/{projectId}/alertPolicies/{alertPolicyId}\n  method: get\n  operationId: getAlertPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/projects/{projectId}/alertPolicies/{alertPolicyId}\n\
  \  method: patch\n  operationId: updateAlertPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/projects/{projectId}/alertPolicies/{alertPolicyId}\n  method: delete\n  operationId: deleteAlertPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/projects/{projectId}/uptimeCheckConfigs\n  method: get\n  operationId: listUptimeCheckConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/projects/{projectId}/uptimeCheckConfigs\n\
  \  method: post\n  operationId: createUptimeCheckConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/projects/{projectId}/notificationChannels\n  method: get\n  operationId: listNotificationChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/projects/{projectId}/notificationChannels\n  method: post\n  operationId: createNotificationChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/projects/{projectId}/metricDescriptors\n\
  \  method: get\n  operationId: listMetricDescriptors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/projects/{projectId}/metricDescriptors\n  method: post\n  operationId: createMetricDescriptor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/projects/{projectId}/groups\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-monitoring/refs/heads/main/agentic-access/google-cloud-monitoring-agentic-access.yml
summary_line: 14 operations · 7 acting
tags:
- Alerting
- Dashboards
- Google Cloud
- Metrics
- Monitoring
- Observability
- SLO
- Uptime
---

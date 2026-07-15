---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 22
api_specs:
- filename: openapi.json
  format: json
  label: Qiskit Runtime Jobs API
  slug: qiskit-runtime-jobs-api
  spec_type: OpenAPI
  url: https://quantum.cloud.ibm.com/api/openapi.json
- filename: ibm-quantum-runtime-backends-openapi.yml
  format: yaml
  label: Qiskit Runtime Backends API
  slug: qiskit-runtime-backends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-quantum/refs/heads/main/openapi/ibm-quantum-runtime-backends-openapi.yml
- filename: ibm-quantum-runtime-sessions-openapi.yml
  format: yaml
  label: Qiskit Runtime Sessions API
  slug: qiskit-runtime-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-quantum/refs/heads/main/openapi/ibm-quantum-runtime-sessions-openapi.yml
- filename: ibm-quantum-runtime-instances-openapi.yml
  format: yaml
  label: Qiskit Runtime Instances API
  slug: qiskit-runtime-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-quantum/refs/heads/main/openapi/ibm-quantum-runtime-instances-openapi.yml
- filename: ibm-quantum-runtime-analytics-openapi.yml
  format: yaml
  label: Qiskit Runtime Analytics API
  slug: qiskit-runtime-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-quantum/refs/heads/main/openapi/ibm-quantum-runtime-analytics-openapi.yml
- filename: ibm-quantum-runtime-versions-openapi.yml
  format: yaml
  label: Qiskit Runtime Versions API
  slug: qiskit-runtime-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-quantum/refs/heads/main/openapi/ibm-quantum-runtime-versions-openapi.yml
consequence_counts:
  read: 22
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ibm Quantum Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'ibm-quantum exposes 30 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ibm-quantum
provider_slug: ibm-quantum
slug: ibm-quantum-agentic-access
source_filename: ibm-quantum-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ibm-quantum-runtime-analytics-openapi.yml, openapi/ibm-quantum-runtime-backends-openapi.yml,\n  openapi/ibm-quantum-runtime-instances-openapi.yml, openapi/ibm-quantum-runtime-jobs-openapi.yml,\n  openapi/ibm-quantum-runtime-sessions-openapi.yml, openapi/ibm-quantum-runtime-versions-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 22\n    acting: 8\n  by_consequence:\n    read: 22\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/workloads\n  method: get\n  operationId: find_instance_workloads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/analytics/usage\n  method: get\n  operationId: analytics_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/usage_grouped\n  method: get\n  operationId: get_usage_analytics_grouped\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/usage_grouped_by_date\n  method: get\n  operationId: get_usage_analytics_grouped_by_date\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/filters\n  method: get\n  operationId: analytics_filters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/backends\n  method:\
  \ get\n  operationId: list_backends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/backends/{id}/properties\n  method: get\n  operationId: get_backend_properties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/backends/{id}/configuration\n  method: get\n  operationId: get_backend_configuration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/backends/{id}/status\n  method: get\n  operationId: get_backend_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/backends/{id}/defaults\n  method: get\n  operationId: get_backend_defaults\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/instance\n  method: get\n  operationId: get_instance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/instances/configuration\n  method: get\n  operationId: get_instance_configuration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/instances/configuration\n  method: put\n  operationId: replace_instance_configuration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{id}\n  method: get\n  operationId:\
  \ get_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/instances/usage\n  method: get\n  operationId: get_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{id}\n  method: get\n  operationId: get_job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{id}\n  method: delete\n  operationId: delete_job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs\n  method: get\n  operationId: list_jobs\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs\n  method: post\n  operationId: create_job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{id}/results\n  method: get\n  operationId: get_job_results_jid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{id}/logs\n  method: get\n  operationId: get_jog_logs_jid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{id}/cancel\n  method: post\n  operationId: cancel_job_jid\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{id}/metrics\n  method: get\n  operationId: get_job_metrics_jid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{id}/tags\n  method: put\n  operationId: replace_job_tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tags\n  method: get\n  operationId: list_tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/sessions\n  method: post\n  operationId: create_session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{id}\n  method: get\n  operationId: get_session\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{id}\n  method: patch\n  operationId: update_session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{id}/close\n  method: delete\n\
  \  operationId: delete_session_close\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/versions\n  method: get\n  operationId: get_versions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibm-quantum/refs/heads/main/agentic-access/ibm-quantum-agentic-access.yml
summary_line: 30 operations · 8 acting
tags: []
---

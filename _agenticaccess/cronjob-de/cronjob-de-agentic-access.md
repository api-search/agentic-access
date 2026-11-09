---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 11
api_specs:
- filename: cronjob-de-benachrichtigungen-api-openapi.yml
  format: yaml
  label: Cronjob.de Benachrichtigungen API
  slug: cronjob-de-benachrichtigungen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronjob-de/openapi/cronjob-de-benachrichtigungen-api-openapi.yml
- filename: cronjob-de-cronjobs-und-heartbeats-api-openapi.yml
  format: yaml
  label: Cronjob.de Cronjobs und Heartbeats API
  slug: cronjob-de-cronjobs-und-heartbeats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronjob-de/openapi/cronjob-de-cronjobs-und-heartbeats-api-openapi.yml
- filename: cronjob-de-server-berwachung-und-ssl-api-openapi.yml
  format: yaml
  label: Cronjob.de Serverüberwachung und SSL API
  slug: cronjob-de-server-berwachung-und-ssl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronjob-de/openapi/cronjob-de-server-berwachung-und-ssl-api-openapi.yml
- filename: cronjob-de-statusseiten-api-openapi.yml
  format: yaml
  label: Cronjob.de Statusseiten API
  slug: cronjob-de-statusseiten-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronjob-de/openapi/cronjob-de-statusseiten-api-openapi.yml
consequence_counts:
  read: 11
  safety-critical: 2
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Cronjob De Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /jobs/{job_id}/active
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /monitors/{monitor_id}/active
operation_count: 28
overview: 'Cronjob.de exposes 28 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 15 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cronjob.de
provider_slug: cronjob-de
slug: cronjob-de-agentic-access
source_filename: cronjob-de-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/cronjob-de-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 11\n    acting: 17\n  by_consequence:\n    read: 11\n    write: 15\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /jobs\n  method: get\n  operationId: list_jobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs\n  method: post\n  operationId: create_job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{job_id}\n  method: get\n  operationId: get_job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{job_id}\n  method: patch\n  operationId: update_job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{job_id}\n  method: delete\n  operationId: delete_job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{job_id}/history\n\
  \  method: get\n  operationId: list_job_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{job_id}/timeline\n  method: get\n  operationId: get_job_timeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{job_id}/active\n  method: put\n  operationId: set_job_active\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /jobs/{job_id}/move\n  method: post\n  operationId: move_job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{job_id}/run\n  method: post\n  operationId: run_job_now\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /heartbeats\n  method: post\n  operationId: create_heartbeat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /failures\n  method: get\n  operationId: list_failures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /folders\n  method: get\n  operationId: list_folders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /folders\n  method: post\n  operationId: create_folder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitors\n  method: get\n  operationId: list_monitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors\n  method: post\n  operationId: create_monitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitors/{monitor_id}\n  method: get\n  operationId: get_monitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/{monitor_id}\n  method: patch\n  operationId: update_monitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitors/{monitor_id}\n  method: delete\n  operationId: delete_monitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitors/{monitor_id}/active\n  method: put\n  operationId: set_monitor_active\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ssl-certificates\n  method: get\n  operationId: list_ssl_certificates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts\n  method: get\n  operationId: list_contacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts\n  method: post\n  operationId: add_contact\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alert-recipients\n  method: put\n  operationId: set_alert_recipients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status-pages\n  method: get\n  operationId: list_status_pages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status-pages\n  method: post\n  operationId: create_status_page\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status-pages/{status_page_id}\n  method: patch\n  operationId: update_status_page\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status-pages/{status_page_id}\n  method: delete\n  operationId: delete_status_page\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/cronjob-de/agentic-access/cronjob-de-agentic-access.yml
summary_line: 28 operations · 17 acting · 2 human-in-the-loop
tags:
- Cronjob
- Scheduling
- Automation
- EU-hosted
---

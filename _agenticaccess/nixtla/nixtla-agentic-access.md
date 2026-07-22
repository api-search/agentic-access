---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 4
api_specs:
- filename: nixtla-openapi-original.json
  format: json
  label: Nixtla Forecast API
  slug: nixtla-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nixtla/refs/heads/main/openapi/nixtla-openapi-original.json
consequence_counts:
  read: 4
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nixtla Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Nixtla exposes 10 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nixtla
provider_slug: nixtla
slug: nixtla-agentic-access
source_filename: nixtla-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/nixtla-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 6\n    connected: 4\n  by_consequence:\n    write: 6\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/forecast\n  method: post\n  operationId: v2_forecast_v2_forecast_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/anomaly_detection\n  method: post\n  operationId: v2_anomaly_detection_v2_anomaly_detection_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/online_anomaly_detection\n  method: post\n  operationId: v2_online_anomaly_detection_v2_online_anomaly_detection_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model_params\n  method: get\n  operationId: get_model_params_model_params_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/cross_validation\n  method: post\n  operationId: v2_cross_validation_v2_cross_validation_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/finetune\n  method: post\n  operationId: v2_finetune_v2_finetune_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/finetuned_models\n  method: get\n  operationId: v2_finetuned_models_v2_finetuned_models_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/finetuned_models/{finetuned_model_id}\n  method: get\n  operationId: v2_finetuned_model_v2_finetuned_models__finetuned_model_id__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/finetuned_models/{finetuned_model_id}\n  method: delete\n  operationId: v2_finetuned_models_delete_v2_finetuned_models__finetuned_model_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validate_api_key\n  method: get\n  operationId: validate_api_key_validate_api_key_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nixtla/refs/heads/main/agentic-access/nixtla-agentic-access.yml
summary_line: 10 operations · 6 acting
tags:
- Company
- Time Series
- Forecasting
- Anomaly Detection
- Machine Learning
- Artificial Intelligence
- Foundation Model
- Predictive Analytics
- Data Science
---

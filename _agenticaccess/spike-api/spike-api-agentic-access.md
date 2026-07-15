---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 22
api_specs:
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Authentication API
  slug: spike-api-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Provider Integrations API
  slug: spike-api-provider-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Provider Records API
  slug: spike-api-provider-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Sleep API
  slug: spike-api-sleep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Workouts API
  slug: spike-api-workouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Time Series API
  slug: spike-api-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Statistics API
  slug: spike-api-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Nutrition AI API
  slug: spike-api-nutrition-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Lab Reports API
  slug: spike-api-lab-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Users API
  slug: spike-api-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike SDK Push API
  slug: spike-api-sdk-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
consequence_counts:
  read: 22
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Spike Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 39
overview: 'Spike exposes 39 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 17 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Spike
provider_slug: spike-api
slug: spike-api-agentic-access
source_filename: spike-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/spike-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    acting: 17\n    connected: 22\n  by_consequence:\n    write: 17\n    read: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/hmac\n  method: post\n  operationId: authHmac\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/client_token\n  method: post\n  operationId: authClientToken\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/pkcs1\n  method: post\n  operationId: authPkcs1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicationinfo\n  method: get\n  operationId: getApplicationInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /userinfo\n  method: get\n  operationId: getUserInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /userproperties\n\
  \  method: get\n  operationId: getUserProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/{provider_slug}/integration/init\n  method: get\n  operationId: initProviderIntegration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/{provider_slug}/integration/init_url\n  method: get\n  operationId: getProviderIntegrationInitUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/{provider_slug}/integration\n  method: delete\n  operationId: deleteProviderIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers/{provider_slug}/integration/callback\n  method: get\n  operationId: providerIntegrationCallback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /queries/provider_records\n  method: get\n  operationId: listProviderRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /queries/provider_records/{record_id}\n  method: get\n  operationId: getProviderRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /queries/provider_record\n  method: post\n  operationId: queryProviderRecordCompat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /queries/sleeps\n  method: get\n  operationId: listSleeps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /queries/sleeps/{sleep_id}\n  method: get\n  operationId: getSleep\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /queries/workouts\n  method: get\n  operationId: listWorkouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /queries/workouts/{workout_id}\n  method: get\n  operationId: getWorkout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /queries/timeseries\n  method: get\n  operationId: queryTimeSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /queries/timeseries/samples\n  method: get\n  operationId: queryTimeSeriesSamples\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /queries/timeseries/split\n  method: get\n  operationId: queryTimeSeriesSplit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /queries/statistics/daily\n  method: get\n  operationId: queryStatisticsDaily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /queries/statistics/interval\n  method: get\n  operationId: queryStatisticsInterval\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /queries/statistics/interpolation\n  method: get\n  operationId: queryStatisticsInterpolation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nutrition_records\n  method: get\n  operationId: listNutritionRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nutrition_records/image\n  method: post\n  operationId: analyzeNutritionImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /nutrition_records/ingredients/label\n  method: post\n  operationId: analyzeNutritionLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /nutrition_records/text\n  method: post\n  operationId: analyzeNutritionText\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /nutrition_records/manual\n  method: post\n  operationId: createManualNutritionRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /nutrition_records/{nutrition_record_id}\n  method: get\n  operationId: getNutritionRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nutrition_records/{nutrition_record_id}\n  method: patch\n  operationId: modifyNutritionRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /nutrition_records/{nutrition_record_id}\n  method: put\n  operationId: replaceNutritionRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /nutrition_records/{nutrition_record_id}\n  method: delete\n  operationId: deleteNutritionRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lab_reports\n  method: get\n  operationId: listLabReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lab_reports\n  method: post\n  operationId: uploadLabReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lab_reports/process\n  method: post\n  operationId: processLabReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lab_reports/{lab_report_id}\n  method: get\n  operationId: getLabReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/apple/push\n  method: post\n  operationId: pushAppleHealth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers/health_connect/push\n  method: post\n  operationId: pushHealthConnect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers/samsung_health_data/push/proto\n  method: post\n  operationId: pushSamsungHealth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/agentic-access/spike-api-agentic-access.yml
summary_line: 39 operations · 17 acting
tags:
- Health Data
- Wearables
- Fitness
- Digital Health
- Data Aggregation
- HIPAA
---

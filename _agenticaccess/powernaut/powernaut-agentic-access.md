---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 16
api_specs:
- filename: powernaut-authentication-api-openapi.yml
  format: yaml
  label: Powernaut authentication API
  slug: powernaut-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-authentication-api-openapi.yml
- filename: powernaut-baselining-api-openapi.yml
  format: yaml
  label: Powernaut baselining API
  slug: powernaut-baselining-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-baselining-api-openapi.yml
- filename: powernaut-creating-bids-api-openapi.yml
  format: yaml
  label: Powernaut creating_bids API
  slug: powernaut-creating-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-creating-bids-api-openapi.yml
- filename: powernaut-events-api-openapi.yml
  format: yaml
  label: Powernaut events API
  slug: powernaut-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-events-api-openapi.yml
- filename: powernaut-getting-forecasts-api-openapi.yml
  format: yaml
  label: Powernaut getting_forecasts API
  slug: powernaut-getting-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-getting-forecasts-api-openapi.yml
- filename: powernaut-historical-data-api-openapi.yml
  format: yaml
  label: Powernaut historical_data API
  slug: powernaut-historical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-historical-data-api-openapi.yml
- filename: powernaut-managing-bids-api-openapi.yml
  format: yaml
  label: Powernaut managing_bids API
  slug: powernaut-managing-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-managing-bids-api-openapi.yml
- filename: powernaut-markets-api-openapi.yml
  format: yaml
  label: Powernaut markets API
  slug: powernaut-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-markets-api-openapi.yml
- filename: powernaut-metrics-api-openapi.yml
  format: yaml
  label: Powernaut metrics API
  slug: powernaut-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-metrics-api-openapi.yml
- filename: powernaut-resources-api-openapi.yml
  format: yaml
  label: Powernaut resources API
  slug: powernaut-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-resources-api-openapi.yml
- filename: powernaut-sensor-data-api-openapi.yml
  format: yaml
  label: Powernaut sensor_data API
  slug: powernaut-sensor-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-sensor-data-api-openapi.yml
- filename: powernaut-sites-api-openapi.yml
  format: yaml
  label: Powernaut sites API
  slug: powernaut-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-sites-api-openapi.yml
- filename: powernaut-uploading-forecasts-api-openapi.yml
  format: yaml
  label: Powernaut uploading_forecasts API
  slug: powernaut-uploading-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-uploading-forecasts-api-openapi.yml
- filename: powernaut-accepting-bids-api-openapi.yml
  format: yaml
  label: Powernaut Accepting Bids API
  slug: powernaut-accepting-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-accepting-bids-api-openapi.yml
consequence_counts:
  read: 16
  safety-critical: 5
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Powernaut Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/connect/sites/{id}/credentials
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/connect/sites/{id}/credentials
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/connect/sites/{id}/credentials/rotate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/connect/sites/{id}/credentials/rotate/cancel
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/connect/sites/{id}/credentials/rotate/complete
operation_count: 38
overview: 'Powernaut exposes 38 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 17 write, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Powernaut
provider_slug: powernaut
slug: powernaut-agentic-access
source_filename: powernaut-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/powernaut-partner-api-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    acting: 22\n    connected: 16\n  by_consequence:\n    write: 17\n    read: 16\n    safety-critical: 5\n  human_in_the_loop_required: 5\noperations:\n- path: /v1/auth/token\n  method: post\n  operationId: GetToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect/sites\n  method: post\n  operationId: CreateSite\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect/sites\n  method: get\n  operationId: FindAllSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/sites/{id}\n  method: get\n  operationId: GetSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/sites/{id}\n  method: patch\n  operationId: UpdateSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/connect/sites/{id}\n  method: delete\n  operationId: RemoveSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect/sites/{id}/baseline\n  method: get\n  operationId: RetrieveBaselineSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/sites/{id}/baseline\n  method: post\n  operationId: BaselineSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /v1/connect/sites/{id}/credentials\n  method: post\n  operationId: SitesController_createCredentials_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/connect/sites/{id}/credentials\n  method: get\n  operationId: SitesController_listCredentials_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/sites/{id}/credentials\n  method: delete\n  operationId: SitesController_revokeCredentials_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/connect/sites/{id}/credentials/rotate\n  method: post\n  operationId: SitesController_startRotation_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/connect/sites/{id}/credentials/rotate/complete\n  method: post\n  operationId: SitesController_completeRotation_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/connect/sites/{id}/credentials/rotate/cancel\n\
  \  method: post\n  operationId: SitesController_cancelRotation_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/connect/sites/{id}/metrics\n  method: get\n  operationId: ActualPowerMetricsSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/sites/{id}/markets\n  method: get\n  operationId: MarketsSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/sites/{id}/sensors\n  method: get\n  operationId: ListSiteSensors\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/sites/{id}/forecast\n  method: get\n  operationId: GetForecastForSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/sites/{id}/forecast\n  method: post\n  operationId: UploadSiteForecast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect/resources\n  method: post\n  operationId: CreateResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/connect/resources\n  method: get\n  operationId: FindAllResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/resources/{id}\n  method: get\n  operationId: GetResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/resources/{id}\n  method: patch\n  operationId: UpdateResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect/resources/{id}\n  method: delete\n  operationId: RemoveResource\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect/resources/{id}/baseline\n  method: post\n  operationId: BaselineResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect/resources/{id}/bid\n  method: post\n  operationId: BidResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect/resources/{id}/activations\n  method:\
  \ get\n  operationId: GetActivationsForResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/resources/{id}/forecast\n  method: get\n  operationId: GetForecastForResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/resources/{id}/forecast\n  method: post\n  operationId: UploadResourceForecast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect/resources/{id}/events\n  method: post\n  operationId: ReportEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect/bids\n  method: get\n  operationId: FindAllBids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/bids/{id}\n  method: get\n  operationId: GetBid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/bids/{id}\n  method: patch\n  operationId: UpdateBid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect/bids/{id}\n  method:\
  \ delete\n  operationId: CancelBid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect/historical-data/upload-url\n  method: post\n  operationId: CreateHistoricalDataUploadUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect/historical-data/{import_id}/confirm\n  method: post\n  operationId: ConfirmHistoricalDataImport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect/sensors/{id}\n  method: get\n  operationId: GetSensor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/sensors/{id}/readings\n  method: get\n  operationId: GetSensorReadings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/agentic-access/powernaut-agentic-access.yml
summary_line: 38 operations · 22 acting · 5 human-in-the-loop
tags:
- Company
- Energy
- Virtual Power Plant
- Distributed Energy Resources
- Energy Trading
- Flexibility
- Forecasting
- Grid
---

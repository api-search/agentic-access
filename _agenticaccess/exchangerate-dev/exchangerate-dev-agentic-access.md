---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 31
api_specs:
- filename: exchangerate-dev-account-api-openapi.yml
  format: yaml
  label: exchangerate-dev Account API
  slug: exchangerate-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-account-api-openapi.yml
- filename: exchangerate-dev-consent-api-openapi.yml
  format: yaml
  label: exchangerate-dev Consent API
  slug: exchangerate-dev-consent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-consent-api-openapi.yml
- filename: exchangerate-dev-convert-api-openapi.yml
  format: yaml
  label: exchangerate-dev Convert API
  slug: exchangerate-dev-convert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-convert-api-openapi.yml
- filename: exchangerate-dev-currencies-api-openapi.yml
  format: yaml
  label: exchangerate-dev Currencies API
  slug: exchangerate-dev-currencies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-currencies-api-openapi.yml
- filename: exchangerate-dev-exchangerate-dev-api-openapi.yml
  format: yaml
  label: exchangerate-dev Exchangerate.dev API
  slug: exchangerate-dev-exchangerate-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-exchangerate-dev-api-openapi.yml
- filename: exchangerate-dev-health-api-openapi.yml
  format: yaml
  label: exchangerate-dev Health API
  slug: exchangerate-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-health-api-openapi.yml
- filename: exchangerate-dev-indices-api-openapi.yml
  format: yaml
  label: exchangerate-dev Indices API
  slug: exchangerate-dev-indices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-indices-api-openapi.yml
- filename: exchangerate-dev-keys-api-openapi.yml
  format: yaml
  label: exchangerate-dev Keys API
  slug: exchangerate-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-keys-api-openapi.yml
- filename: exchangerate-dev-latest-api-openapi.yml
  format: yaml
  label: exchangerate-dev Latest API
  slug: exchangerate-dev-latest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-latest-api-openapi.yml
- filename: exchangerate-dev-official-api-openapi.yml
  format: yaml
  label: exchangerate-dev Official API
  slug: exchangerate-dev-official-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-official-api-openapi.yml
- filename: exchangerate-dev-range-api-openapi.yml
  format: yaml
  label: exchangerate-dev Range API
  slug: exchangerate-dev-range-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-range-api-openapi.yml
- filename: exchangerate-dev-rate-api-openapi.yml
  format: yaml
  label: exchangerate-dev Rate API
  slug: exchangerate-dev-rate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-rate-api-openapi.yml
- filename: exchangerate-dev-status-api-openapi.yml
  format: yaml
  label: exchangerate-dev Status API
  slug: exchangerate-dev-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-status-api-openapi.yml
- filename: exchangerate-dev-webhooks-api-openapi.yml
  format: yaml
  label: exchangerate-dev Webhooks API
  slug: exchangerate-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-webhooks-api-openapi.yml
- filename: exchangerate-dev-time-series-api-openapi.yml
  format: yaml
  label: exchangerate-dev Time Series API
  slug: exchangerate-dev-time-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-time-series-api-openapi.yml
consequence_counts:
  physical: 4
  read: 31
  safety-critical: 1
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Exchangerate Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/keys
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/account/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/account/checkout-session
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/account/provision
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/account/webhooks/{endpoint_id}/test
operation_count: 46
overview: 'exchangerate-dev exposes 46 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read, 10 write, 4 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: exchangerate-dev
provider_slug: exchangerate-dev
slug: exchangerate-dev-agentic-access
source_filename: exchangerate-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/exchangerate-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 46\n  by_action_class:\n    connected: 31\n    acting: 15\n  by_consequence:\n    read: 31\n    write: 10\n    physical: 4\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: status_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/currencies\n  method: get\n  operationId: currencies_v1_currencies_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/latest/{path_base}\n  method: get\n  operationId: latest_v1_latest__path_base__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/latest\n  method: get\n  operationId: latest_v1_latest_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/convert/{from_ccy}/{to_ccy}/{amount}\n  method: get\n  operationId: convert_v1_convert__from_ccy___to_ccy___amount__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/convert/{from_ccy}/{to_ccy}\n\
  \  method: get\n  operationId: convert_v1_convert__from_ccy___to_ccy__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/convert\n  method: post\n  operationId: convert_batch_v1_convert_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/range\n  method: get\n  operationId: range_endpoint_v1_range_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/timeseries\n  method: get\n  operationId: timeseries_endpoint_v1_timeseries_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/indices/{index_slug}\n  method: get\n  operationId: index_snapshot_v1_indices__index_slug__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/indices/{index_slug}/timeseries\n  method: get\n  operationId: index_timeseries_v1_indices__index_slug__timeseries_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/provision\n  method: post\n  operationId: provision_v1_account_provision_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/account/checkout\n  method: post\n  operationId: account_checkout_v1_account_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/checkout-session\n  method: post\n  operationId: account_checkout_session_v1_account_checkout_session_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account\n  method: get\n  operationId: account_v1_account_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: delete\n  operationId: delete_account_v1_account_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/usage/daily\n  method: get\n  operationId: account_usage_daily_v1_account_usage_daily_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/keys\n  method: get\n  operationId: list_named_keys_v1_account_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/keys\n  method:\
  \ post\n  operationId: manage_named_key_v1_account_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/rotate\n  method: post\n  operationId: rotate_key_v1_keys_rotate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys\n  method: delete\n  operationId: revoke_key_v1_keys_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/consent\n  method: post\n  operationId: record_consent_v1_consent_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/rate/{slug}\n  method: get\n  operationId: rate_v1_rate__slug__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{date}/{path_base}\n  method: get\n  operationId: historical_v1__date___path_base__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{date}\n  method: get\n  operationId: historical_v1__date__get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/official/evidence/{lookup_id}\n  method: get\n  operationId: evidence_v1_official_evidence__lookup_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/official\n  method: get\n  operationId: countries_v1_official_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/official/changes\n  method: get\n  operationId: changes_v1_official_changes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/official/{country}\n  method: get\n  operationId: country_v1_official__country__get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/official/{country}/{rate_type}\n  method: get\n  operationId: table_info_v1_official__country___rate_type__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/official/{country}/{rate_type}/rate/{base}/{quote}\n  method: get\n  operationId: rate_v1_official__country___rate_type__rate__base___quote__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/official/{country}/{rate_type}/convert/{base}/{quote}/{amount}\n  method: get\n  operationId: convert_v1_official__country___rate_type__convert__base___quote___amount__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/official/{country}/{rate_type}/convert\n  method: post\n  operationId: convert_batch_v1_official__country___rate_type__convert_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/official/{country}/{rate_type}/period/{month}\n  method: get\n  operationId: period_v1_official__country___rate_type__period__month__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/official/{country}/{rate_type}/gain-loss\n  method: post\n  operationId: gain_loss_v1_official__country___rate_type__gain_loss_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/official/{country}/{rate_type}/rates.xlsx\n  method: get\n  operationId: rates_v1_official__country___rate_type__rates_xlsx_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/official/{country}/{rate_type}/rates.csv\n  method: get\n  operationId: rates_v1_official__country___rate_type__rates_csv_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/official/{country}/{rate_type}/rates\n  method: get\n  operationId: rates_v1_official__country___rate_type__rates_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/official/{country}/{rate_type}/publications\n\
  \  method: get\n  operationId: publications_v1_official__country___rate_type__publications_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/official/{country}/{rate_type}/publications/{publication_id}\n  method: get\n  operationId: publication_v1_official__country___rate_type__publications__publication_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/webhooks\n  method: get\n  operationId: list_webhooks_v1_account_webhooks_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/webhooks\n  method: post\n  operationId: create_webhook_v1_account_webhooks_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/webhooks/{endpoint_id}\n  method: delete\n  operationId: delete_webhook_v1_account_webhooks__endpoint_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/webhooks/{endpoint_id}/rotate-secret\n  method: post\n  operationId: rotate_secret_v1_account_webhooks__endpoint_id__rotate_secret_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/account/webhooks/{endpoint_id}/test\n  method: post\n  operationId: send_test_v1_account_webhooks__endpoint_id__test_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/exchangerate-dev/agentic-access/exchangerate-dev-agentic-access.yml
summary_line: 46 operations · 15 acting · 1 human-in-the-loop
tags:
- Company
- Finance
- Currency
- Exchange Rates
---

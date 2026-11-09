---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 24
api_specs:
- filename: anteproof-com-account-api-openapi.yml
  format: yaml
  label: Anteproof Account API
  slug: anteproof-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-account-api-openapi.yml
- filename: anteproof-com-anchor-api-openapi.yml
  format: yaml
  label: Anteproof Anchor API
  slug: anteproof-com-anchor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-anchor-api-openapi.yml
- filename: anteproof-com-billing-api-openapi.yml
  format: yaml
  label: Anteproof Billing API
  slug: anteproof-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-billing-api-openapi.yml
- filename: anteproof-com-calibration-api-openapi.yml
  format: yaml
  label: Anteproof Calibration API
  slug: anteproof-com-calibration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-calibration-api-openapi.yml
- filename: anteproof-com-chain-api-openapi.yml
  format: yaml
  label: Anteproof Chain API
  slug: anteproof-com-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-chain-api-openapi.yml
- filename: anteproof-com-coverage-preview-api-openapi.yml
  format: yaml
  label: Anteproof Coverage Preview API
  slug: anteproof-com-coverage-preview-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-coverage-preview-api-openapi.yml
- filename: anteproof-com-digest-api-openapi.yml
  format: yaml
  label: Anteproof Digest API
  slug: anteproof-com-digest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-digest-api-openapi.yml
- filename: anteproof-com-entities-api-openapi.yml
  format: yaml
  label: Anteproof Entities API
  slug: anteproof-com-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-entities-api-openapi.yml
- filename: anteproof-com-forecasts-api-openapi.yml
  format: yaml
  label: Anteproof Forecasts API
  slug: anteproof-com-forecasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-forecasts-api-openapi.yml
- filename: anteproof-com-freshness-api-openapi.yml
  format: yaml
  label: Anteproof Freshness API
  slug: anteproof-com-freshness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-freshness-api-openapi.yml
- filename: anteproof-com-me-api-openapi.yml
  format: yaml
  label: Anteproof Me API
  slug: anteproof-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-me-api-openapi.yml
- filename: anteproof-com-proof-api-openapi.yml
  format: yaml
  label: Anteproof Proof API
  slug: anteproof-com-proof-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-proof-api-openapi.yml
- filename: anteproof-com-questions-api-openapi.yml
  format: yaml
  label: Anteproof Questions API
  slug: anteproof-com-questions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-questions-api-openapi.yml
- filename: anteproof-com-risk-api-openapi.yml
  format: yaml
  label: Anteproof Risk API
  slug: anteproof-com-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-risk-api-openapi.yml
- filename: anteproof-com-stats-api-openapi.yml
  format: yaml
  label: Anteproof Stats API
  slug: anteproof-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-stats-api-openapi.yml
- filename: anteproof-com-support-api-openapi.yml
  format: yaml
  label: Anteproof Support API
  slug: anteproof-com-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-support-api-openapi.yml
consequence_counts:
  physical: 1
  read: 24
  safety-critical: 1
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Anteproof Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/me/api-keys/{key_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/checkout
operation_count: 36
overview: 'Anteproof exposes 36 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read, 10 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Anteproof
provider_slug: anteproof-com
slug: anteproof-com-agentic-access
source_filename: anteproof-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/anteproof-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    connected: 24\n    acting: 12\n  by_consequence:\n    read: 24\n    write: 10\n    safety-critical: 1\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/account/config\n  method: get\n  operationId: account_config_v1_account_config_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me\n  method: get\n  operationId: me_v1_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/me/watchlist\n  method: get\n  operationId: watchlist_v1_me_watchlist_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me/watchlist\n  method: post\n  operationId: watch_v1_me_watchlist_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/watchlist/import\n  method: post\n  operationId: import_watchlist_v1_me_watchlist_import_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/me/watchlist/pending\n  method: get\n  operationId: watchlist_pending_v1_me_watchlist_pending_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me/watchlist/pending\n  method: delete\n  operationId: clear_pending_v1_me_watchlist_pending_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/watchlist/pending/{pending_id}\n  method: delete\n  operationId: delete_pending_v1_me_watchlist_pending__pending_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/watchlist/{entity_id}\n  method: delete\n  operationId: unwatch_v1_me_watchlist__entity_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/api-keys\n  method: get\n  operationId: api_keys_v1_me_api_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me/api-keys\n  method: post\n  operationId: create_api_key_v1_me_api_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /v1/me/api-keys/{key_id}\n  method: delete\n  operationId: revoke_api_key_v1_me_api_keys__key_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/me/alerts\n  method: get\n  operationId: get_alerts_v1_me_alerts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me/alerts\n  method: put\n  operationId: put_alerts_v1_me_alerts_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/checkout\n  method: post\n  operationId: checkout_v1_billing_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/portal\n  method: get\n  operationId: portal_v1_billing_portal_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/webhooks/stripe\n  method: post\n  operationId: stripe_webhook_v1_billing_webhooks_stripe_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/support\n  method: post\n  operationId: submit_v1_support_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/entities\n  method: get\n  operationId: search_entities_v1_entities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/forecasts\n  method: get\n  operationId: list_forecasts_v1_forecasts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/questions/{question_id}\n  method: get\n  operationId: question_detail_v1_questions__question_id__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities/{entity_id}\n  method: get\n  operationId: entity_detail_v1_entities__entity_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/risk\n  method: get\n  operationId: dependency_risk_v1_risk_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/risk/batch\n  method: post\n  operationId: risk_batch_endpoint_v1_risk_batch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/coverage-preview\n  method: get\n  operationId: coverage_preview_endpoint_v1_coverage_preview_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/risk/top\n  method: get\n  operationId: top_risk_v1_risk_top_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities/{entity_id}/risk\n  method: get\n  operationId: entity_risk_v1_entities__entity_id__risk_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calibration\n  method: get\n  operationId: calibration_v1_calibration_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calibration/families\n\
  \  method: get\n  operationId: calibration_by_family_v1_calibration_families_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/proof\n  method: get\n  operationId: proof_record_v1_proof_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/head\n  method: get\n  operationId: chain_head_v1_chain_head_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/rows\n  method: get\n  operationId: chain_rows_v1_chain_rows_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/anchor/latest\n  method: get\n  operationId: anchor_latest_v1_anchor_latest_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stats\n  method: get\n  operationId: stats_v1_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/freshness\n  method: get\n  operationId: freshness_v1_freshness_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/digest\n  method: get\n  operationId: digest_v1_digest_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/anteproof-com/agentic-access/anteproof-com-agentic-access.yml
summary_line: 36 operations · 12 acting · 1 human-in-the-loop
tags:
- Dependency
- Risk Management
- Analytics
- Open Source
- Software
---

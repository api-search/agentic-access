---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 30
api_specs:
- filename: polystrike-xyz-bulk-api-openapi.yml
  format: yaml
  label: polystrike-xyz Bulk API
  slug: polystrike-xyz-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/polystrike-xyz/openapi/polystrike-xyz-bulk-api-openapi.yml
- filename: polystrike-xyz-history-api-openapi.yml
  format: yaml
  label: polystrike-xyz History API
  slug: polystrike-xyz-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/polystrike-xyz/openapi/polystrike-xyz-history-api-openapi.yml
- filename: polystrike-xyz-metadata-api-openapi.yml
  format: yaml
  label: polystrike-xyz Metadata API
  slug: polystrike-xyz-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/polystrike-xyz/openapi/polystrike-xyz-metadata-api-openapi.yml
- filename: polystrike-xyz-performance-api-openapi.yml
  format: yaml
  label: polystrike-xyz Performance API
  slug: polystrike-xyz-performance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/polystrike-xyz/openapi/polystrike-xyz-performance-api-openapi.yml
- filename: polystrike-xyz-portfolio-api-openapi.yml
  format: yaml
  label: polystrike-xyz Portfolio API
  slug: polystrike-xyz-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/polystrike-xyz/openapi/polystrike-xyz-portfolio-api-openapi.yml
- filename: polystrike-xyz-predictions-api-openapi.yml
  format: yaml
  label: polystrike-xyz Predictions API
  slug: polystrike-xyz-predictions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/polystrike-xyz/openapi/polystrike-xyz-predictions-api-openapi.yml
- filename: polystrike-xyz-signals-api-openapi.yml
  format: yaml
  label: polystrike-xyz Signals API
  slug: polystrike-xyz-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/polystrike-xyz/openapi/polystrike-xyz-signals-api-openapi.yml
- filename: polystrike-xyz-system-api-openapi.yml
  format: yaml
  label: polystrike-xyz System API
  slug: polystrike-xyz-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/polystrike-xyz/openapi/polystrike-xyz-system-api-openapi.yml
- filename: polystrike-xyz-usage-api-openapi.yml
  format: yaml
  label: polystrike-xyz Usage API
  slug: polystrike-xyz-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/polystrike-xyz/openapi/polystrike-xyz-usage-api-openapi.yml
consequence_counts:
  read: 30
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Polystrike Xyz Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 32
overview: 'polystrike-xyz exposes 32 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: polystrike-xyz
provider_slug: polystrike-xyz
slug: polystrike-xyz-agentic-access
source_filename: polystrike-xyz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/polystrike-xyz-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 30\n    acting: 2\n  by_consequence:\n    read: 30\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/meta/elon\n  method: get\n  operationId: get_elon_meta_api_v1_meta_elon_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/meta/cruz\n  method: get\n  operationId: get_cruz_meta_api_v1_meta_cruz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /api/v1/meta/trump\n  method: get\n  operationId: get_trump_meta_api_v1_meta_trump_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signals/elon\n  method: get\n  operationId: get_elon_signals_api_v1_signals_elon_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signals/cruz\n  method: get\n  operationId: get_cruz_signals_api_v1_signals_cruz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signals/trump\n  method: get\n  operationId: get_trump_signals_api_v1_signals_trump_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/meta/crypto\n  method: get\n  operationId: get_crypto_meta_api_v1_meta_crypto_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/meta/elon/tweets\n  method: get\n  operationId: get_tweets_api_v1_meta_elon_tweets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/meta/cruz/tweets\n  method: get\n  operationId: get_cruz_tweets_api_v1_meta_cruz_tweets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/meta/trump/posts\n  method: get\n  operationId: get_trump_posts_api_v1_meta_trump_posts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/prediction/elon\n  method: get\n  operationId: get_elon_prediction_api_v1_prediction_elon_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prediction/cruz\n  method: get\n  operationId: get_cruz_prediction_api_v1_prediction_cruz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prediction/trump\n  method: get\n  operationId: get_trump_prediction_api_v1_prediction_trump_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/portfolio/elon\n  method: get\n  operationId: get_portfolio_analysis_api_v1_portfolio_elon_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /api/v1/portfolio/elon/rebalancing\n  method: get\n  operationId: get_rebalancing_summary_api_v1_portfolio_elon_rebalancing_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/health\n  method: get\n  operationId: health_check_api_v1_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/waitlist\n  method: post\n  operationId: waitlist_api_v1_waitlist_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/keys/free\n  method: post\n  operationId: issue_free_key_api_v1_keys_free_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/performance/overview\n  method: get\n  operationId: get_performance_overview_api_v1_performance_overview_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/performance/history\n  method: get\n  operationId: get_performance_history_api_v1_performance_history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/history/{user}/counter\n  method: get\n  operationId: counter_history_api_v1_history__user__counter_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/history/{user}/prices\n  method: get\n  operationId: price_history_api_v1_history__user__prices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/history/{user}/books\n  method: get\n  operationId: book_history_api_v1_history__user__books_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/history/{user}/tweets\n  method: get\n  operationId: tweet_history_api_v1_history__user__tweets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bulk/public\n  method: get\n  operationId: list_public_api_v1_bulk_public_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bulk/public/{table}/{date}/{file}\n  method: get\n  operationId: get_public_file_api_v1_bulk_public__table___date___file__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bulk/{user}\n  method: get\n  operationId: list_user_files_api_v1_bulk__user__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bulk/{user}/{table}/{date}/{file}\n  method: get\n  operationId: get_user_file_api_v1_bulk__user___table___date___file__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage/summary\n  method: get\n  operationId: get_usage_summary_api_v1_usage_summary_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage/by-endpoint\n  method: get\n  operationId: get_usage_by_endpoint_api_v1_usage_by_endpoint_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage/errors\n  method: get\n  operationId: get_error_logs_api_v1_usage_errors_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage/stats\n  method: get\n  operationId: get_usage_stats_api_v1_usage_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/polystrike-xyz/agentic-access/polystrike-xyz-agentic-access.yml
summary_line: 32 operations · 2 acting
tags:
- Company
- Finance
- Data
- Prediction Market
- Cryptocurrency
---

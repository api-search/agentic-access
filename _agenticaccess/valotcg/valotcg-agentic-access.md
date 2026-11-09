---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 18
api_specs:
- filename: valotcg-analysis-api-openapi.yml
  format: yaml
  label: Valo.Data Analysis API
  slug: valotcg-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valotcg/openapi/valotcg-analysis-api-openapi.yml
- filename: valotcg-cards-api-openapi.yml
  format: yaml
  label: Valo.Data Cards API
  slug: valotcg-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valotcg/openapi/valotcg-cards-api-openapi.yml
- filename: valotcg-editions-api-openapi.yml
  format: yaml
  label: Valo.Data Editions API
  slug: valotcg-editions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valotcg/openapi/valotcg-editions-api-openapi.yml
- filename: valotcg-games-api-openapi.yml
  format: yaml
  label: Valo.Data Games API
  slug: valotcg-games-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valotcg/openapi/valotcg-games-api-openapi.yml
- filename: valotcg-sealed-api-openapi.yml
  format: yaml
  label: Valo.Data Sealed API
  slug: valotcg-sealed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valotcg/openapi/valotcg-sealed-api-openapi.yml
- filename: valotcg-usage-api-openapi.yml
  format: yaml
  label: Valo.Data Usage API
  slug: valotcg-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valotcg/openapi/valotcg-usage-api-openapi.yml
consequence_counts:
  read: 18
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Valotcg Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Valo.Data exposes 20 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Valo.Data
provider_slug: valotcg
slug: valotcg-agentic-access
source_filename: valotcg-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/valotcg-data-v1-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 18\n    acting: 2\n  by_consequence:\n    read: 18\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /data/v1/games\n  method: get\n  operationId: get_games_data_v1_games_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/games/{game}/rarities\n  method: get\n  operationId: get_game_rarities_data_v1_games__game__rarities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /data/v1/editions\n  method: get\n  operationId: search_editions_data_v1_editions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/cards\n  method: get\n  operationId: search_cards_data_v1_cards_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/cards/{card_id}\n  method: get\n  operationId: read_card_data_v1_cards__card_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/cards/{card_id}/prices\n  method: get\n  operationId: read_card_prices_data_v1_cards__card_id__prices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /data/v1/cards/batch\n  method: post\n  operationId: batch_prices_data_v1_cards_batch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/cards/{card_id}/price-history\n  method: get\n  operationId: read_card_price_history_data_v1_cards__card_id__price_history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/sealed\n  method: get\n  operationId: search_sealed_data_v1_sealed_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/sealed/{sealed_id}\n  method: get\n  operationId: read_sealed_data_v1_sealed__sealed_id__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/sealed/{sealed_id}/prices\n  method: get\n  operationId: read_sealed_prices_data_v1_sealed__sealed_id__prices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/sealed/{sealed_id}/price-history\n  method: get\n  operationId: read_sealed_price_history_data_v1_sealed__sealed_id__price_history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/analysis/identify\n  method: get\n  operationId: identify_data_v1_analysis_identify_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/analysis/cards/{card_id}/summary\n\
  \  method: get\n  operationId: card_price_summary_data_v1_analysis_cards__card_id__summary_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/analysis/sealed/{sealed_id}/summary\n  method: get\n  operationId: sealed_price_summary_data_v1_analysis_sealed__sealed_id__summary_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/analysis/compare\n  method: post\n  operationId: compare_prices_data_v1_analysis_compare_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/analysis/top-movers\n  method: get\n  operationId: read_top_movers_data_v1_analysis_top_movers_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/analysis/top-priced\n  method: get\n  operationId: read_top_priced_data_v1_analysis_top_priced_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/analysis/editions/{edition_id}/overview\n  method: get\n  operationId: read_edition_overview_data_v1_analysis_editions__edition_id__overview_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /developer/v1/usage\n  method: get\n  operationId: get_usage_developer_v1_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/valotcg/agentic-access/valotcg-agentic-access.yml
summary_line: 20 operations · 2 acting
tags:
- Trading Card Games
- Pricing Data
- Vision
---

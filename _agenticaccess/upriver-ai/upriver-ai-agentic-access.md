---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 34
api_specs:
- filename: upriver-ai-account-api-openapi.yml
  format: yaml
  label: upriver-ai Account API
  slug: upriver-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upriver-ai/openapi/upriver-ai-account-api-openapi.yml
- filename: upriver-ai-audience-api-openapi.yml
  format: yaml
  label: upriver-ai Audience API
  slug: upriver-ai-audience-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upriver-ai/openapi/upriver-ai-audience-api-openapi.yml
- filename: upriver-ai-brands-api-openapi.yml
  format: yaml
  label: upriver-ai Brands API
  slug: upriver-ai-brands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upriver-ai/openapi/upriver-ai-brands-api-openapi.yml
- filename: upriver-ai-breakout-feeds-api-openapi.yml
  format: yaml
  label: upriver-ai Breakout Feeds API
  slug: upriver-ai-breakout-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upriver-ai/openapi/upriver-ai-breakout-feeds-api-openapi.yml
- filename: upriver-ai-breakout-topics-api-openapi.yml
  format: yaml
  label: upriver-ai Breakout Topics API
  slug: upriver-ai-breakout-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upriver-ai/openapi/upriver-ai-breakout-topics-api-openapi.yml
- filename: upriver-ai-creators-api-openapi.yml
  format: yaml
  label: upriver-ai Creators API
  slug: upriver-ai-creators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upriver-ai/openapi/upriver-ai-creators-api-openapi.yml
- filename: upriver-ai-images-api-openapi.yml
  format: yaml
  label: upriver-ai Images API
  slug: upriver-ai-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upriver-ai/openapi/upriver-ai-images-api-openapi.yml
- filename: upriver-ai-products-api-openapi.yml
  format: yaml
  label: upriver-ai Products API
  slug: upriver-ai-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upriver-ai/openapi/upriver-ai-products-api-openapi.yml
- filename: upriver-ai-sponsorships-api-openapi.yml
  format: yaml
  label: upriver-ai Sponsorships API
  slug: upriver-ai-sponsorships-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upriver-ai/openapi/upriver-ai-sponsorships-api-openapi.yml
- filename: upriver-ai-taxonomy-api-openapi.yml
  format: yaml
  label: upriver-ai Taxonomy API
  slug: upriver-ai-taxonomy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upriver-ai/openapi/upriver-ai-taxonomy-api-openapi.yml
- filename: upriver-ai-trends-api-openapi.yml
  format: yaml
  label: upriver-ai Trends API
  slug: upriver-ai-trends-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upriver-ai/openapi/upriver-ai-trends-api-openapi.yml
- filename: upriver-ai-trends-radar-beta-api-openapi.yml
  format: yaml
  label: upriver-ai Trends Radar (Beta) API
  slug: upriver-ai-trends-radar-beta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upriver-ai/openapi/upriver-ai-trends-radar-beta-api-openapi.yml
consequence_counts:
  read: 34
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Upriver Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 43
overview: 'upriver-ai exposes 43 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 34 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: upriver-ai
provider_slug: upriver-ai
slug: upriver-ai-agentic-access
source_filename: upriver-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/upriver-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    acting: 9\n    connected: 34\n  by_consequence:\n    write: 9\n    read: 34\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/brand/research\n  method: post\n  operationId: brand_research\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/brand/products\n  method: post\n  operationId: brand_product\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/brand/product\n  method: post\n  operationId: brand_product_detail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/creators\n  method: get\n  operationId: creator_get_by_url\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/creators/{creator_id}\n  method: get\n  operationId: creator_get_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /v1/creators/batch\n  method: post\n  operationId: creator_batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/creators/search\n  method: post\n  operationId: creator_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/creators/similar\n  method: post\n  operationId: creator_similar_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/audience_insights\n\
  \  method: post\n  operationId: audience_insights_v3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/catalogs/{catalog_id}/match\n  method: post\n  operationId: match_catalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sponsors\n  method: get\n  operationId: sponsors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sponsors/{sponsor_id}/channels\n  method: get\n  operationId: sponsor_channels_list\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sponsorships\n  method: get\n  operationId: sponsorships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/trends/broad\n  method: post\n  operationId: trends_broad_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/trends/{trend_id}\n  method: get\n  operationId: get_trend_by_id_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/trends/{trend_id}/media\n  method: get\n  operationId:\
  \ trends_media_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/trends/{trend_id}/playback\n  method: get\n  operationId: trends_playback_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/trends/{trend_id}/similar\n  method: get\n  operationId: trends_similar_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/trends/{trend_id}/traction\n  method: get\n  operationId: get_trend_traction_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/radar\n  method: get\n  operationId: list_radar_beta\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/radar/breakouts\n  method: get\n  operationId: list_radar_breakouts_beta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/radar/facets\n  method: get\n  operationId: get_radar_facets_beta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/radar/items/{item_id}\n  method: get\n  operationId: get_radar_item_beta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/radar/search\n  method: post\n  operationId: search_radar_beta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v2/radar/topics\n  method: get\n  operationId: list_radar_topics_beta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/radar/trends\n  method: get\n  operationId: list_radar_trends_beta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities/breakout\n  method: get\n  operationId: list_breakout_entities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities/breakout/tags\n  method: get\n  operationId: list_breakout_entity_tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities/{entity_id}/breakout\n  method: get\n  operationId: get_breakout_entity\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topics/breakout\n  method: get\n  operationId: list_breakout_topics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topics/breakout/metadata\n  method: get\n  operationId: get_breakout_metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topics/breakout/narratives\n  method: get\n  operationId: list_narratives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topics/breakout/narratives/{narrative_id}\n  method: get\n  operationId: get_narrative\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topics/breakout/search\n  method: post\n  operationId: search_breakout_topics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topics/breakout/similar\n  method: post\n  operationId: find_similar_topics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topics/breakout/{topic_id}\n  method: get\n  operationId: get_breakout_topic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topics/breakout/{topic_id}/story\n  method: get\n  operationId: get_breakout_topic_story_view\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/categories/search\n  method: post\n  operationId: search_categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/media_categories\n  method: get\n  operationId: media_categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/breakout/feeds\n  method: get\n  operationId: list_private_breakout_feeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/breakout/feeds/{feed_slug}\n  method: get\n  operationId: get_private_breakout_feed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/images/download\n  method:\
  \ post\n  operationId: download_image_bytes_v1_images_download_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: get_usage_v1_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/upriver-ai/agentic-access/upriver-ai-agentic-access.yml
summary_line: 43 operations · 9 acting
tags:
- Artificial Intelligence
- Marketing
- Data
- Creators
- Brands
- Trends
- Sponsorship
---

---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 15
api_specs:
- filename: antismi-media-authentication-api-openapi.yml
  format: yaml
  label: AntiSMI Authentication API
  slug: antismi-media-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antismi-media/openapi/antismi-media-authentication-api-openapi.yml
- filename: antismi-media-digest-api-openapi.yml
  format: yaml
  label: AntiSMI Digest API
  slug: antismi-media-digest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antismi-media/openapi/antismi-media-digest-api-openapi.yml
- filename: antismi-media-favicon-ico-api-openapi.yml
  format: yaml
  label: AntiSMI Favicon.ico API
  slug: antismi-media-favicon-ico-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antismi-media/openapi/antismi-media-favicon-ico-api-openapi.yml
- filename: antismi-media-health-api-openapi.yml
  format: yaml
  label: AntiSMI Health API
  slug: antismi-media-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antismi-media/openapi/antismi-media-health-api-openapi.yml
- filename: antismi-media-icon-png-api-openapi.yml
  format: yaml
  label: AntiSMI Icon.png API
  slug: antismi-media-icon-png-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antismi-media/openapi/antismi-media-icon-png-api-openapi.yml
- filename: antismi-media-metrics-api-openapi.yml
  format: yaml
  label: AntiSMI Metrics API
  slug: antismi-media-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antismi-media/openapi/antismi-media-metrics-api-openapi.yml
- filename: antismi-media-news-api-openapi.yml
  format: yaml
  label: AntiSMI News API
  slug: antismi-media-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antismi-media/openapi/antismi-media-news-api-openapi.yml
- filename: antismi-media-reference-api-openapi.yml
  format: yaml
  label: AntiSMI Reference API
  slug: antismi-media-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antismi-media/openapi/antismi-media-reference-api-openapi.yml
- filename: antismi-media-russian-news-archive-api-api-openapi.yml
  format: yaml
  label: AntiSMI Russian News Archive API
  slug: antismi-media-russian-news-archive-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antismi-media/openapi/antismi-media-russian-news-archive-api-api-openapi.yml
consequence_counts:
  read: 15
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Antismi Media Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'AntiSMI exposes 22 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AntiSMI
provider_slug: antismi-media
slug: antismi-media-agentic-access
source_filename: antismi-media-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/antismi-media-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 15\n    acting: 7\n  by_consequence:\n    read: 15\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /favicon.ico\n  method: get\n  operationId: favicon_favicon_ico_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /icon.png\n  method: get\n  operationId: icon_icon_png_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n \
  \ operationId: root__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics\n  method: get\n  operationId: metrics_metrics_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news/{news_id}\n  method: get\n  operationId: get_news_by_id_news__news_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news/search\n  method: post\n  operationId: search_news_news_search_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news/similarity_search\n  method: post\n  operationId: similarity_search_news_similarity_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /news/vector_search\n  method: post\n  operationId: vector_search_news_vector_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /news/topic_timeline\n  method: post\n  operationId: topic_timeline_news_topic_timeline_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /categories\n  method: get\n  operationId: get_categories_categories_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agencies\n  method: get\n  operationId: get_agencies_agencies_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/limits\n  method: get\n  operationId: get_limits_auth_limits_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/test-key\n  method: post\n  operationId: test_api_key_auth_test_key_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /news/digest\n  method: post\n  operationId: create_digest_news_digest_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /news/digest/categories\n  method: get\n  operationId: get_available_categories_news_digest_categories_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news/digest/historical\n  method: post\n  operationId: create_historical_digest_news_digest_historical_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /news/wordcloud\n  method: post\n  operationId: generate_wordcloud_news_wordcloud_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /news/wordcloud_data\n  method: post\n  operationId: get_wordcloud_data_news_wordcloud_data_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news/trends\n  method: post\n  operationId: get_trends_news_trends_post\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news/wordcloud_zscore\n  method: post\n  operationId: get_wordcloud_zscore_news_wordcloud_zscore_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news/notion_trend\n  method: post\n  operationId: get_notion_trend_news_notion_trend_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/antismi-media/agentic-access/antismi-media-agentic-access.yml
summary_line: 22 operations · 7 acting
tags:
- News
- Artificial Intelligence
- Search
- Media
- Russian
---

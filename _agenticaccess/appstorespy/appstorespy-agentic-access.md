---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 26
api_specs:
- filename: appstorespy-app-store-api-openapi.yml
  format: yaml
  label: AppstoreSpy App Store API
  slug: appstorespy-app-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appstorespy/refs/heads/main/openapi/appstorespy-app-store-api-openapi.yml
- filename: appstorespy-events-api-openapi.yml
  format: yaml
  label: AppstoreSpy Events API
  slug: appstorespy-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appstorespy/refs/heads/main/openapi/appstorespy-events-api-openapi.yml
- filename: appstorespy-google-play-api-openapi.yml
  format: yaml
  label: AppstoreSpy Google Play API
  slug: appstorespy-google-play-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appstorespy/refs/heads/main/openapi/appstorespy-google-play-api-openapi.yml
- filename: appstorespy-jobs-api-openapi.yml
  format: yaml
  label: AppstoreSpy Jobs API
  slug: appstorespy-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appstorespy/refs/heads/main/openapi/appstorespy-jobs-api-openapi.yml
- filename: appstorespy-search-filter-v-2-api-openapi.yml
  format: yaml
  label: AppstoreSpy Search Filter v.2 API
  slug: appstorespy-search-filter-v-2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appstorespy/refs/heads/main/openapi/appstorespy-search-filter-v-2-api-openapi.yml
- filename: appstorespy-suggestions-api-openapi.yml
  format: yaml
  label: AppstoreSpy Suggestions API
  slug: appstorespy-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appstorespy/refs/heads/main/openapi/appstorespy-suggestions-api-openapi.yml
consequence_counts:
  read: 26
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Appstorespy Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 33
overview: 'AppstoreSpy exposes 33 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AppstoreSpy
provider_slug: appstorespy
slug: appstorespy-agentic-access
source_filename: appstorespy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: generated\nsource: openapi/appstorespy-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 26\n    acting: 7\n  by_consequence:\n    read: 26\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /ios/apps/{id}\n  method: get\n  operationId: get_app_details_ios_apps__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ios/apps\n  method: get\n  operationId: get_app_search_ios_apps_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /ios/apps/{id}/reviews\n  method: get\n  operationId: get_reviews_ios_apps__id__reviews_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ios/apps/query\n  method: post\n  operationId: get_filter_search_ios_apps_query_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ios/apps/similar\n  method: post\n  operationId: get_similar_ios_apps_similar_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ios/apps/summary\n\
  \  method: post\n  operationId: get_summary_ios_apps_summary_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ios/apps/{id}/recrawl\n  method: get\n  operationId: get_recrawl_ios_apps__id__recrawl_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ios/estimates\n  method: get\n  operationId: get_apps_estimates_ios_estimates_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ios/info/countries\n  method: get\n  operationId: get_play_app_countries_ios_info_countries_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ios/info/languages\n  method: get\n  operationId: get_play_app_languages_ios_info_languages_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ios/developers/{id}\n  method: get\n  operationId: get_developer_ios_developers__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ios/developers\n  method: get\n  operationId: dev_search_ios_developers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ios/developers/{id}/estimates\n  method: get\n  operationId: get_apps_estimates_ios_developers__id__estimates_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ios/rankings\n  method: get\n  operationId: get_ios_rankings_ios_rankings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/search\n  method: get\n  operationId: get_search_jobs_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/search\n  method: post\n  operationId: create_search_jobs_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /play/apps\n  method: get\n  operationId: get_app_search_play_apps_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /play/apps/{id}/reviews\n  method: get\n  operationId: get_reviews_play_apps__id__reviews_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /play/apps/{id}/recrawl\n  method: get\n  operationId: get_recrawl_play_apps__id__recrawl_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /play/apps/query\n  method: post\n  operationId: get_filter_search_play_apps_query_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /play/apps/similar\n  method: post\n  operationId: get_similar_play_apps_similar_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /play/apps/summary\n  method: post\n  operationId: get_summary_play_apps_summary_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /play/apps/{id}\n  method: get\n  operationId: get_app_details_play_apps__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /play/info/countries\n\
  \  method: get\n  operationId: get_play_app_countries_play_info_countries_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /play/info/languages\n  method: get\n  operationId: get_play_app_languages_play_info_languages_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /play/developers/{id}\n  method: get\n  operationId: get_developer_play_developers__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /play/developers\n  method: get\n  operationId: dev_search_play_developers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /play/developers/{id}/estimates\n\
  \  method: get\n  operationId: get_apps_estimates_play_developers__id__estimates_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /play/estimates\n  method: get\n  operationId: get_apps_estimates_play_estimates_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /play/apps/{id}/installs_daily\n  method: get\n  operationId: get_apps_installs_daily_play_apps__id__installs_daily_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /play/suggestions\n  method: get\n  operationId: get_suggests_play_suggestions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /play/liveops\n\
  \  method: get\n  operationId: get_events_play_liveops_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /play/rankings\n  method: get\n  operationId: get_play_rankings_play_rankings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appstorespy/refs/heads/main/agentic-access/appstorespy-agentic-access.yml
summary_line: 33 operations · 7 acting
tags:
- mobile-apps
- app-store-optimization
- market-intelligence
- app-analytics
- google-play
- apple-app-store
- reviews-and-ratings
- download-revenue-estimates
- marketing
---

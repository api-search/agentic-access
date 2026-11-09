---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 22
api_specs:
- filename: socially-run-attributions-api-openapi.yml
  format: yaml
  label: socially-run Attributions API
  slug: socially-run-attributions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socially-run/openapi/socially-run-attributions-api-openapi.yml
- filename: socially-run-dossiers-api-openapi.yml
  format: yaml
  label: socially-run Dossiers API
  slug: socially-run-dossiers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socially-run/openapi/socially-run-dossiers-api-openapi.yml
- filename: socially-run-emails-api-openapi.yml
  format: yaml
  label: socially-run Emails API
  slug: socially-run-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socially-run/openapi/socially-run-emails-api-openapi.yml
- filename: socially-run-jobs-api-openapi.yml
  format: yaml
  label: socially-run Jobs API
  slug: socially-run-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socially-run/openapi/socially-run-jobs-api-openapi.yml
- filename: socially-run-platforms-api-openapi.yml
  format: yaml
  label: socially-run Platforms API
  slug: socially-run-platforms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socially-run/openapi/socially-run-platforms-api-openapi.yml
- filename: socially-run-posts-api-openapi.yml
  format: yaml
  label: socially-run Posts API
  slug: socially-run-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socially-run/openapi/socially-run-posts-api-openapi.yml
- filename: socially-run-profiles-api-openapi.yml
  format: yaml
  label: socially-run Profiles API
  slug: socially-run-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socially-run/openapi/socially-run-profiles-api-openapi.yml
- filename: socially-run-resolve-api-openapi.yml
  format: yaml
  label: socially-run Resolve API
  slug: socially-run-resolve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socially-run/openapi/socially-run-resolve-api-openapi.yml
- filename: socially-run-search-api-openapi.yml
  format: yaml
  label: socially-run Search API
  slug: socially-run-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socially-run/openapi/socially-run-search-api-openapi.yml
- filename: socially-run-trending-api-openapi.yml
  format: yaml
  label: socially-run Trending API
  slug: socially-run-trending-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socially-run/openapi/socially-run-trending-api-openapi.yml
- filename: socially-run-usage-api-openapi.yml
  format: yaml
  label: socially-run Usage API
  slug: socially-run-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socially-run/openapi/socially-run-usage-api-openapi.yml
- filename: socially-run-usernames-api-openapi.yml
  format: yaml
  label: socially-run Usernames API
  slug: socially-run-usernames-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socially-run/openapi/socially-run-usernames-api-openapi.yml
- filename: socially-run-web-api-openapi.yml
  format: yaml
  label: socially-run Web API
  slug: socially-run-web-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socially-run/openapi/socially-run-web-api-openapi.yml
- filename: socially-run-webhooks-api-openapi.yml
  format: yaml
  label: socially-run Webhooks API
  slug: socially-run-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socially-run/openapi/socially-run-webhooks-api-openapi.yml
consequence_counts:
  read: 22
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Socially Run Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'socially-run exposes 30 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: socially-run
provider_slug: socially-run
slug: socially-run-agentic-access
source_filename: socially-run-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/socially-run-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    acting: 8\n    connected: 22\n  by_consequence:\n    write: 8\n    read: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /resolve\n  method: post\n  operationId: resolve_target_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /intelligence/aggregate\n  method: post\n  operationId: aggregate_intelligence_post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platforms\n  method: get\n  operationId: list_platforms_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/lookup\n  method: post\n  operationId: lookup_profile_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/{platform}/{handle}\n  method: get\n  operationId: get_profile_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/batch\n  method: post\n  operationId: lookup_profiles_batch_post\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /posts/lookup\n  method: post\n  operationId: lookup_post_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/read\n  method: post\n  operationId: read_website_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /web/og\n  method: post\n  operationId: fetch_og_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}\n  method: get\n  operationId: get_job_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}/hits\n  method: get\n  operationId: list_job_hits_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}/cancel\n  method: post\n  operationId: cancel_job_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usernames/search\n  method: post\n  operationId: search_username_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usernames/sites\n  method: get\n  operationId: list_username_sites_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emails/lookup\n  method: post\n  operationId: lookup_email_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dossiers\n  method: post\n  operationId: create_dossier_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trending\n  method: get\n  operationId: list_trending_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/youtube\n  method: get\n  operationId: search_youtube_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/news\n  method: get\n  operationId: search_news_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/instagram\n  method: get\n  operationId: search_instagram_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/tiktok\n  method: get\n  operationId: search_tiktok_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/instagram-hashtag\n  method: get\n  operationId: search_instagram_hashtag_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /search/github\n  method: get\n  operationId: search_github_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  operationId: get_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: get_webhook_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: put\n  operationId: set_webhook_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /webhooks\n  method: delete\n  operationId: delete_webhook_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/test\n  method: post\n  operationId: test_webhook_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/deliveries\n  method: get\n  operationId: list_webhook_deliveries_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attributions\n  method: get\n  operationId: get_attributions_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/socially-run/agentic-access/socially-run-agentic-access.yml
summary_line: 30 operations · 8 acting
tags:
- Social Media
- Data API
- JSON
- MCP
- AI Agents
---

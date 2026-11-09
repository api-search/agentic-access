---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 38
api_specs:
- filename: creatordb-app-ai-search-api-openapi.yml
  format: yaml
  label: creatordb-app AI Search API
  slug: creatordb-app-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatordb-app/openapi/creatordb-app-ai-search-api-openapi.yml
- filename: creatordb-app-general-operations-api-openapi.yml
  format: yaml
  label: creatordb-app General Operations API
  slug: creatordb-app-general-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatordb-app/openapi/creatordb-app-general-operations-api-openapi.yml
- filename: creatordb-app-instagram-api-openapi.yml
  format: yaml
  label: creatordb-app Instagram API
  slug: creatordb-app-instagram-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatordb-app/openapi/creatordb-app-instagram-api-openapi.yml
- filename: creatordb-app-sponsor-api-openapi.yml
  format: yaml
  label: creatordb-app Sponsor API
  slug: creatordb-app-sponsor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatordb-app/openapi/creatordb-app-sponsor-api-openapi.yml
- filename: creatordb-app-tiktok-api-openapi.yml
  format: yaml
  label: creatordb-app Tik Tok API
  slug: creatordb-app-tiktok-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatordb-app/openapi/creatordb-app-tiktok-api-openapi.yml
- filename: creatordb-app-youtube-api-openapi.yml
  format: yaml
  label: creatordb-app YouTube API
  slug: creatordb-app-youtube-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatordb-app/openapi/creatordb-app-youtube-api-openapi.yml
consequence_counts:
  read: 38
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Creatordb App Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 42
overview: 'creatordb-app exposes 42 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 38 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: creatordb-app
provider_slug: creatordb-app
slug: creatordb-app-agentic-access
source_filename: creatordb-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/creatordb-app-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 38\n    acting: 4\n  by_consequence:\n    read: 38\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /usage\n  method: get\n  operationId: getApiUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nls\n  method: post\n  operationId: getNLS\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /youtube/search\n  method: post\n  operationId: searchYoutube\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /youtube/submitCreators\n  method: post\n  operationId: submitYoutubeCreators\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /youtube/profile\n  method: post\n  operationId: getYoutubeProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /youtube/contact\n  method: post\n  operationId: getYoutubeContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /youtube/performance\n  method: post\n\
  \  operationId: getYoutubePerformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /youtube/performance-history\n  method: get\n  operationId: getYoutubePerformanceHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /youtube/audience\n  method: post\n  operationId: getYoutubeAudience\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /youtube/content-detail\n  method: post\n  operationId: getYoutubeContentDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /youtube/sponsorship\n  method: post\n  operationId: getYoutubeSponsorship\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /youtube/topics\n  method: get\n  operationId: getYoutubeTopics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /youtube/niches\n  method: get\n  operationId: getYoutubeNiches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /youtube/subtitles/meta\n  method: get\n  operationId: getYoutubeSubtitleMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /youtube/subtitles/download\n  method: get\n  operationId: getYoutubeSubtitleDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /instagram/search\n  method: post\n  operationId: searchInstagram\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/submitCreators\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instagram/profile\n  method: post\n  operationId: getInstagramProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/contact\n  method: post\n  operationId: getInstagramContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /instagram/performance\n  method: post\n  operationId: getInstagramPerformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/performance-history\n  method: get\n  operationId: getInstagramPerformanceHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/audience\n  method: post\n  operationId: getInstagramAudience\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/content-detail\n  method: post\n  operationId: getInstagramContentDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/sponsorship\n\
  \  method: post\n  operationId: getInstagramSponsorship\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/niches\n  method: get\n  operationId: getInstagramNiches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiktok/search\n  method: post\n  operationId: searchTiktok\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiktok/submitCreators\n  method: post\n  operationId: submitTiktokCreators\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /tiktok/profile\n  method: post\n  operationId: getTiktokProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiktok/contact\n  method: post\n  operationId: getTiktokContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiktok/performance\n  method: post\n  operationId: getTiktokPerformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiktok/performance-history\n  method: get\n  operationId: getTiktokPerformanceHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiktok/audience\n  method: post\n  operationId: getTiktokAudience\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiktok/content-detail\n  method: post\n  operationId: getTiktokContentDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiktok/niches\n  method: get\n  operationId: getTiktokNiches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sponsor/search\n  method: post\n  operationId: searchSponsor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sponsor/submit\n  method: post\n  operationId: submitSponsor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sponsor/information\n  method: get\n  operationId: getSponsorInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sponsor/list\n  method: get\n  operationId: getSponsorList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sponsor/creators\n  method: get\n  operationId: getSponsorCreators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sponsor/performance\n  method: get\n  operationId: getSponsorPerformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /sponsor/audience\n  method: get\n  operationId: getSponsorAudience\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sponsor/summary\n  method: get\n  operationId: getSponsorSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/creatordb-app/agentic-access/creatordb-app-agentic-access.yml
summary_line: 42 operations · 4 acting
tags:
- Company
- Creator Data
- Influencer Marketing
- Analytics
- Asia
---

---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 32
api_specs:
- filename: emplifi-io-ads-api-openapi.yml
  format: yaml
  label: Emplifi Ads API
  slug: emplifi-io-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-ads-api-openapi.yml
- filename: emplifi-io-assets-api-openapi.yml
  format: yaml
  label: Emplifi Assets API
  slug: emplifi-io-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-assets-api-openapi.yml
- filename: emplifi-io-care-api-openapi.yml
  format: yaml
  label: Emplifi Care API
  slug: emplifi-io-care-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-care-api-openapi.yml
- filename: emplifi-io-community-api-openapi.yml
  format: yaml
  label: Emplifi Community API
  slug: emplifi-io-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-community-api-openapi.yml
- filename: emplifi-io-listening-api-openapi.yml
  format: yaml
  label: Emplifi Listening API
  slug: emplifi-io-listening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-listening-api-openapi.yml
- filename: emplifi-io-posts-api-openapi.yml
  format: yaml
  label: Emplifi Posts API
  slug: emplifi-io-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-posts-api-openapi.yml
- filename: emplifi-io-profile-metrics-api-openapi.yml
  format: yaml
  label: Emplifi Profile Metrics API
  slug: emplifi-io-profile-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-profile-metrics-api-openapi.yml
- filename: emplifi-io-reference-api-openapi.yml
  format: yaml
  label: Emplifi Reference API
  slug: emplifi-io-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-reference-api-openapi.yml
consequence_counts:
  read: 32
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Socialbakers Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 41
overview: 'Emplifi exposes 41 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Emplifi
provider_slug: emplifi-io
slug: socialbakers-agentic-access
source_filename: socialbakers-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/socialbakers-ads-api-openapi.yml, openapi/socialbakers-assets-api-openapi.yml,\n  openapi/socialbakers-care-api-openapi.yml, openapi/socialbakers-community-api-openapi.yml,\n  openapi/socialbakers-listening-api-openapi.yml, openapi/socialbakers-posts-api-openapi.yml,\n  openapi/socialbakers-profile-metrics-api-openapi.yml, openapi/socialbakers-reference-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 41\n  by_action_class:\n    connected: 32\n    acting: 9\n  by_consequence:\n    read: 32\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /3/ads/content\n  method: get\n  operationId: getAdsContent\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/ads/metrics\n  method: post\n  operationId: getAdsMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/collections\n  method: get\n  operationId: listCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/collections\n  method: post\n  operationId: createCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /3/collections/{id}\n  method: put\n  operationId: editCollection\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /3/collections/{id}\n  method: delete\n  operationId: deleteCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /3/collections/{id}/archive\n  method: post\n  operationId: archiveCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /3/collections/{id}/restore\n  method: post\n\
  \  operationId: restoreCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /3/assets\n  method: get\n  operationId: getAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/assets/upload\n  method: post\n  operationId: uploadAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /3/assets/{id}\n  method: put\n  operationId: editAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /3/assets/{id}\n  method: delete\n  operationId: deleteAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /3/care/cases\n  method: get\n  operationId: getCareCases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/care/messages\n  method: get\n  operationId: getCareMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/community/content\n\
  \  method: get\n  operationId: getCommunityContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/community/content/labeling\n  method: post\n  operationId: labelCommunityContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /3/community/metrics\n  method: post\n  operationId: getCommunityMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/listening/content\n  method: get\n  operationId: getListeningContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /3/listening/metrics\n  method: post\n  operationId: getListeningMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/facebook/page/posts\n  method: post\n  operationId: getFacebookPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/instagram/profile/posts\n  method: post\n  operationId: getInstagramPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/youtube/profile/videos\n  method: post\n  operationId: getYoutubeVideos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/twitter/profile/tweets\n  method: post\n  operationId:\
  \ getTwitterTweets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/linkedin/page/posts\n  method: post\n  operationId: getLinkedinPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/pinterest/profile/posts\n  method: post\n  operationId: getPinterestPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/tiktok/profile/posts\n  method: post\n  operationId: getTiktokPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/snapchat/profile/posts\n  method: post\n  operationId: getSnapchatPosts\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/facebook/metrics\n  method: post\n  operationId: getFacebookMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/instagram/metrics\n  method: post\n  operationId: getInstagramMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/twitter/metrics\n  method: post\n  operationId: getTwitterMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/youtube/metrics\n  method: post\n  operationId: getYoutubeMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/linkedin/metrics\n\
  \  method: post\n  operationId: getLinkedinMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/pinterest/metrics\n  method: post\n  operationId: getPinterestMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/tiktok/metrics\n  method: post\n  operationId: getTiktokMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/aggregated-metrics\n  method: post\n  operationId: getAggregatedMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/{network}/profiles\n  method: get\n  operationId: listProfiles\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/profile/labels\n  method: get\n  operationId: getProfileLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/post/labels\n  method: get\n  operationId: getPostLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/post/label-groups\n  method: get\n  operationId: getPostLabelGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/listening/queries\n  method: get\n  operationId: getListeningQueries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/ads/accounts\n\
  \  method: post\n  operationId: listAdAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/agentic-access/socialbakers-agentic-access.yml
summary_line: 41 operations · 9 acting
tags:
- Company
- Marketing
- Social Media
- Analytics
- Social Media Analytics
- Social Listening
- Marketing Analytics
- Digital Asset Management
- Customer Care
- Emplifi
---

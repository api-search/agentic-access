---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 23
api_specs:
- filename: tiktok-ad-groups-api-openapi.yml
  format: yaml
  label: TikTok Ad Groups API
  slug: tiktok-ad-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-ad-groups-api-openapi.yml
- filename: tiktok-ads-api-openapi.yml
  format: yaml
  label: TikTok Ads API
  slug: tiktok-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-ads-api-openapi.yml
- filename: tiktok-audiences-api-openapi.yml
  format: yaml
  label: TikTok Audiences API
  slug: tiktok-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-audiences-api-openapi.yml
- filename: tiktok-campaigns-api-openapi.yml
  format: yaml
  label: TikTok Campaigns API
  slug: tiktok-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-campaigns-api-openapi.yml
- filename: tiktok-data-portability-api-openapi.yml
  format: yaml
  label: TikTok Data Portability API
  slug: tiktok-data-portability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-data-portability-api-openapi.yml
- filename: tiktok-finance-api-openapi.yml
  format: yaml
  label: TikTok Finance API
  slug: tiktok-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-finance-api-openapi.yml
- filename: tiktok-logistics-api-openapi.yml
  format: yaml
  label: TikTok Logistics API
  slug: tiktok-logistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-logistics-api-openapi.yml
- filename: tiktok-orders-api-openapi.yml
  format: yaml
  label: TikTok Orders API
  slug: tiktok-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-orders-api-openapi.yml
- filename: tiktok-products-api-openapi.yml
  format: yaml
  label: TikTok Products API
  slug: tiktok-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-products-api-openapi.yml
- filename: tiktok-reporting-api-openapi.yml
  format: yaml
  label: TikTok Reporting API
  slug: tiktok-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-reporting-api-openapi.yml
- filename: tiktok-oauth-api-openapi.yml
  format: yaml
  label: TikTok OAuth API
  slug: tiktok-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-oauth-api-openapi.yml
- filename: tiktok-post-api-openapi.yml
  format: yaml
  label: TikTok Post API
  slug: tiktok-post-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-post-api-openapi.yml
- filename: tiktok-research-comments-api-openapi.yml
  format: yaml
  label: TikTok Research Comments API
  slug: tiktok-research-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-research-comments-api-openapi.yml
- filename: tiktok-research-social-api-openapi.yml
  format: yaml
  label: TikTok Research Social API
  slug: tiktok-research-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-research-social-api-openapi.yml
- filename: tiktok-research-users-api-openapi.yml
  format: yaml
  label: TikTok Research Users API
  slug: tiktok-research-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-research-users-api-openapi.yml
- filename: tiktok-research-videos-api-openapi.yml
  format: yaml
  label: TikTok Research Videos API
  slug: tiktok-research-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-research-videos-api-openapi.yml
- filename: tiktok-user-api-openapi.yml
  format: yaml
  label: TikTok User API
  slug: tiktok-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-user-api-openapi.yml
- filename: tiktok-video-api-openapi.yml
  format: yaml
  label: TikTok Video API
  slug: tiktok-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/openapi/tiktok-video-api-openapi.yml
consequence_counts:
  read: 23
  safety-critical: 1
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Tiktok Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/oauth/revoke/
operation_count: 37
overview: 'TikTok exposes 37 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read, 13 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TikTok
provider_slug: tiktok
slug: tiktok-agentic-access
source_filename: tiktok-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/tiktok-ad-groups-api-openapi.yml, openapi/tiktok-ads-api-openapi.yml, openapi/tiktok-audiences-api-openapi.yml,\n  openapi/tiktok-campaigns-api-openapi.yml, openapi/tiktok-data-portability-api-openapi.yml,\n  openapi/tiktok-finance-api-openapi.yml, openapi/tiktok-for-developers-oauth-api-openapi.yml,\n  openapi/tiktok-for-developers-post-api-openapi.yml, openapi/tiktok-for-developers-research-comments-api-openapi.yml,\n  openapi/tiktok-for-developers-research-social-api-openapi.yml, openapi/tiktok-for-developers-research-users-api-openapi.yml,\n  openapi/tiktok-for-developers-research-videos-api-openapi.yml, openapi/tiktok-for-developers-user-api-openapi.yml,\n  openapi/tiktok-for-developers-video-api-openapi.yml, openapi/tiktok-logistics-api-openapi.yml,\n  openapi/tiktok-orders-api-openapi.yml, openapi/tiktok-products-api-openapi.yml, openapi/tiktok-reporting-api-openapi.yml\ndescription: Recommended x-agentic-access\
  \ execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 23\n    acting: 14\n  by_consequence:\n    read: 23\n    write: 13\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /open_api/v1.3/adgroup/get/\n  method: get\n  operationId: getAdGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open_api/v1.3/adgroup/create/\n  method: post\n  operationId: createAdGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /open_api/v1.3/ad/get/\n  method: get\n  operationId: getAds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open_api/v1.3/ad/create/\n  method: post\n  operationId: createAd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open_api/v1.3/dmp/custom_audience/list/\n  method: get\n  operationId: listCustomAudiences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open_api/v1.3/campaign/get/\n  method: get\n  operationId: getCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /open_api/v1.3/campaign/create/\n  method: post\n  operationId: createCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open_api/v1.3/campaign/update/\n  method: post\n  operationId: updateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/data_portability/task/create/\n  method: post\n  operationId: createDataPortabilityTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/data_portability/task/status/\n  method: post\n  operationId: getDataPortabilityTaskStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /finance/202309/payments\n  method: get\n  operationId: listPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/oauth/token/\n  method: post\n  operationId: exchangeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/oauth/token/refresh/\n\
  \  method: post\n  operationId: refreshToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/oauth/revoke/\n  method: post\n  operationId: revokeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/post/publish/video/init/\n  method: post\n  operationId: initVideoPublish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/post/publish/status/fetch/\n  method: post\n  operationId: getPublishStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/post/publish/inbox/video/init/\n  method: post\n  operationId: initInboxVideoUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/post/publish/creator_info/query/\n  method: post\n  operationId: queryCreatorInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/research/video/comment/list/\n  method: post\n  operationId: listVideoComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/research/user/followers/\n  method: post\n  operationId: listUserFollowers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/research/user/following/\n  method: post\n  operationId: listUserFollowing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/research/user/info/\n  method: post\n  operationId: queryResearchUserInfo\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/research/video/query/\n  method: post\n  operationId: queryResearchVideos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/research/user/liked_videos/\n  method: post\n  operationId: listUserLikedVideos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/research/user/pinned_videos/\n  method: post\n  operationId: listUserPinnedVideos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/research/user/reposted_videos/\n  method: post\n  operationId: listUserRepostedVideos\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/user/info/\n  method: get\n  operationId: getUserInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/video/list/\n  method: post\n  operationId: listVideos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/video/query/\n  method: post\n  operationId: queryVideos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logistics/202309/orders/{order_id}/shipping_documents\n  method: get\n  operationId: getShippingDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order/202309/orders\n\
  \  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order/202309/orders/{order_id}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/202309/products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/202309/products/{product_id}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/202309/products/{product_id}\n  method: put\n  operationId: updateProduct\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/202309/products/upload_files\n  method: post\n  operationId: uploadProductFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open_api/v1.3/report/integrated/get/\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiktok/refs/heads/main/agentic-access/tiktok-agentic-access.yml
summary_line: 37 operations · 14 acting · 1 human-in-the-loop
tags:
- TikTok
- Advertising
- Commerce
- Content
- E-Commerce
- Social Media
- Video
---

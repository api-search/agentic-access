---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 16
api_specs:
- filename: facebook-business-manager-ad-accounts-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Accounts API
  slug: facebook-business-manager-ad-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-accounts-api-openapi.yml
- filename: facebook-business-manager-ad-creatives-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Creatives API
  slug: facebook-business-manager-ad-creatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-creatives-api-openapi.yml
- filename: facebook-business-manager-ad-images-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Images API
  slug: facebook-business-manager-ad-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-images-api-openapi.yml
- filename: facebook-business-manager-ad-sets-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Sets API
  slug: facebook-business-manager-ad-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-sets-api-openapi.yml
- filename: facebook-business-manager-ads-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ads API
  slug: facebook-business-manager-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ads-api-openapi.yml
- filename: facebook-business-manager-campaigns-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Campaigns API
  slug: facebook-business-manager-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-campaigns-api-openapi.yml
- filename: facebook-business-manager-comments-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Comments API
  slug: facebook-business-manager-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-comments-api-openapi.yml
- filename: facebook-business-manager-custom-audiences-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Custom Audiences API
  slug: facebook-business-manager-custom-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-custom-audiences-api-openapi.yml
- filename: facebook-business-manager-insights-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Insights API
  slug: facebook-business-manager-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-insights-api-openapi.yml
- filename: facebook-business-manager-page-insights-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Page Insights API
  slug: facebook-business-manager-page-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-page-insights-api-openapi.yml
- filename: facebook-business-manager-pages-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Pages API
  slug: facebook-business-manager-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-pages-api-openapi.yml
- filename: facebook-business-manager-photos-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Photos API
  slug: facebook-business-manager-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-photos-api-openapi.yml
- filename: facebook-business-manager-posts-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Posts API
  slug: facebook-business-manager-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-posts-api-openapi.yml
- filename: facebook-business-manager-videos-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Videos API
  slug: facebook-business-manager-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-videos-api-openapi.yml
consequence_counts:
  read: 16
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Facebook Business Manager Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 33
overview: 'Facebook Business Manager exposes 33 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 17 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Facebook Business Manager
provider_slug: facebook-business-manager
slug: facebook-business-manager-agentic-access
source_filename: facebook-business-manager-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/facebook-marketing-openapi.yml, openapi/facebook-pages-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 16\n    acting: 17\n  by_consequence:\n    read: 16\n    write: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /act_{ad_account_id}/campaigns\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /act_{ad_account_id}/campaigns\n  method: post\n  operationId: createCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{campaign_id}\n  method: get\n  operationId: getCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{campaign_id}\n  method: post\n  operationId: updateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{campaign_id}\n  method: delete\n  operationId: deleteCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /act_{ad_account_id}/adsets\n  method: get\n  operationId: listAdSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /act_{ad_account_id}/adsets\n  method: post\n  operationId: createAdSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{ad_set_id}\n  method: get\n  operationId: getAdSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ad_set_id}\n  method: post\n  operationId: updateAdSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /act_{ad_account_id}/ads\n  method: get\n  operationId: listAds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /act_{ad_account_id}/ads\n  method: post\n  operationId: createAd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{ad_id}\n  method: get\n  operationId: getAd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /act_{ad_account_id}/adcreatives\n\
  \  method: get\n  operationId: listAdCreatives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /act_{ad_account_id}/adcreatives\n  method: post\n  operationId: createAdCreative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /act_{ad_account_id}\n  method: get\n  operationId: getAdAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /act_{ad_account_id}/customaudiences\n  method: get\n  operationId: listCustomAudiences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /act_{ad_account_id}/customaudiences\n  method: post\n  operationId: createCustomAudience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /act_{ad_account_id}/insights\n  method: get\n  operationId: getAdAccountInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{campaign_id}/insights\n  method: get\n  operationId: getCampaignInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /act_{ad_account_id}/adimages\n  method: post\n  operationId: uploadAdImage\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{page_id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{page_id}/feed\n  method: get\n  operationId: getPageFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{page_id}/feed\n  method: post\n  operationId: createPagePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /{post_id}\n  method: get\n  operationId: getPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{post_id}\n  method: post\n  operationId: updatePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{post_id}\n  method: delete\n  operationId: deletePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{post_id}/comments\n  method: get\n  operationId: getPostComments\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{post_id}/comments\n  method: post\n  operationId: createComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{comment_id}\n  method: delete\n  operationId: deleteComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{page_id}/photos\n  method: post\n  operationId: uploadPagePhoto\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{page_id}/videos\n  method: post\n  operationId: uploadPageVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{page_id}/insights\n  method: get\n  operationId: getPageInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{page_id}/subscribed_apps\n  method: post\n  operationId: subscribePageApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/agentic-access/facebook-business-manager-agentic-access.yml
summary_line: 33 operations · 17 acting
tags:
- Advertising
- Analytics
- Business Management
- Marketing
- Social Media
- Messaging
- Commerce
- Agents
- MCP
- Webhooks
---

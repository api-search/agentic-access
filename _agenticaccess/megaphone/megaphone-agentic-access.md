---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 15
api_specs:
- filename: megaphone-openapi.yml
  format: yaml
  label: Megaphone Networks API
  slug: megaphone-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/openapi/megaphone-openapi.yml
- filename: megaphone-openapi.yml
  format: yaml
  label: Megaphone Podcasts API
  slug: megaphone-podcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/openapi/megaphone-openapi.yml
- filename: megaphone-openapi.yml
  format: yaml
  label: Megaphone Episodes API
  slug: megaphone-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/openapi/megaphone-openapi.yml
- filename: megaphone-openapi.yml
  format: yaml
  label: Megaphone Campaigns and Orders API
  slug: megaphone-campaigns-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/openapi/megaphone-openapi.yml
- filename: megaphone-openapi.yml
  format: yaml
  label: Megaphone Direct Sales API v2
  slug: megaphone-direct-sales-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/openapi/megaphone-openapi.yml
- filename: megaphone-openapi.yml
  format: yaml
  label: Megaphone Metrics and Impressions Export API
  slug: megaphone-metrics-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/openapi/megaphone-openapi.yml
consequence_counts:
  read: 15
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Megaphone Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Megaphone exposes 22 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Megaphone
provider_slug: megaphone
slug: megaphone-agentic-access
source_filename: megaphone-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/megaphone-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 15\n    acting: 7\n  by_consequence:\n    read: 15\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /networks/{network_id}\n  method: get\n  operationId: getNetwork\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networks/{network_id}/podcasts\n  method: get\n  operationId: listPodcasts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networks/{network_id}/podcasts\n\
  \  method: post\n  operationId: createPodcast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /networks/{network_id}/podcasts/{podcast_id}\n  method: get\n  operationId: getPodcast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networks/{network_id}/podcasts/{podcast_id}\n  method: put\n  operationId: updatePodcast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /networks/{network_id}/podcasts/{podcast_id}\n  method:\
  \ delete\n  operationId: deletePodcast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /networks/{network_id}/podcasts/{podcast_id}/episodes\n  method: get\n  operationId: listEpisodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networks/{network_id}/podcasts/{podcast_id}/episodes\n  method: post\n  operationId: createEpisode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /networks/{network_id}/podcasts/{podcast_id}/episodes/{episode_id}\n\
  \  method: get\n  operationId: getEpisode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networks/{network_id}/podcasts/{podcast_id}/episodes/{episode_id}\n  method: put\n  operationId: updateEpisode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /networks/{network_id}/podcasts/{podcast_id}/episodes/{episode_id}\n  method: delete\n  operationId: deleteEpisode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/campaigns\n\
  \  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/campaigns/{campaign_id}/orders\n  method: get\n  operationId: listCampaignOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}/advertisements\n  method: get\n  operationId: listOrderAdvertisements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/advertisers\n  method: get\n  operationId: listAdvertisersV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/advertisers\n  method: post\n  operationId: createAdvertiserV2\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/campaigns\n  method: get\n  operationId: listCampaignsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orders\n  method: get\n  operationId: listOrdersV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets\n  method: get\n  operationId: listAssetsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/targeting\n  method: get\n  operationId: getTargetingOptionsV2\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics_export\n  method: get\n  operationId: exportMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /impressions_export\n  method: get\n  operationId: exportImpressions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/megaphone/refs/heads/main/agentic-access/megaphone-agentic-access.yml
summary_line: 22 operations · 7 acting
tags:
- Podcasting
- Podcast Hosting
- Advertising
- Ad Monetization
- Dynamic Ad Insertion
- Media
- Spotify
---

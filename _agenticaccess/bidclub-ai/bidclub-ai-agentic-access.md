---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 18
api_specs:
- filename: bidclub-ai-dl-api-openapi.yml
  format: yaml
  label: BidClub Dl API
  slug: bidclub-ai-dl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidclub-ai/openapi/bidclub-ai-dl-api-openapi.yml
- filename: bidclub-ai-episodes-api-openapi.yml
  format: yaml
  label: BidClub Episodes API
  slug: bidclub-ai-episodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidclub-ai/openapi/bidclub-ai-episodes-api-openapi.yml
- filename: bidclub-ai-feed-index-api-openapi.yml
  format: yaml
  label: BidClub Feed Index API
  slug: bidclub-ai-feed-index-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidclub-ai/openapi/bidclub-ai-feed-index-api-openapi.yml
- filename: bidclub-ai-pitch-api-openapi.yml
  format: yaml
  label: BidClub Pitch API
  slug: bidclub-ai-pitch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidclub-ai/openapi/bidclub-ai-pitch-api-openapi.yml
- filename: bidclub-ai-search-api-openapi.yml
  format: yaml
  label: BidClub Search API
  slug: bidclub-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidclub-ai/openapi/bidclub-ai-search-api-openapi.yml
- filename: bidclub-ai-shows-api-openapi.yml
  format: yaml
  label: BidClub Shows API
  slug: bidclub-ai-shows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidclub-ai/openapi/bidclub-ai-shows-api-openapi.yml
consequence_counts:
  read: 18
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bidclub Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'BidClub exposes 22 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BidClub
provider_slug: bidclub-ai
slug: bidclub-ai-agentic-access
source_filename: bidclub-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/bidclub-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 18\n    acting: 4\n  by_consequence:\n    read: 18\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/pitch/feed\n  method: get\n  operationId: getPitchFeedPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pitch/feed\n  method: options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pitch/auth/request\n  method: post\n  operationId:\
  \ requestPitchAdminOtp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/pitch/auth/verify\n  method: post\n  operationId: verifyPitchAdminOtp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/pitch/auth/logout\n  method: post\n  operationId: logoutPitchAdmin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/pitch/tracking\n  method: post\n  operationId: importPitchTrackingHandles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/shows\n  method: get\n  operationId: listShows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/shows\n  method: options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/episodes\n  method: get\n  operationId: listEpisodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/episodes\n  method: options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/episodes/{slug}\n  method: get\n  operationId: getEpisode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/episodes/{slug}\n  method: options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search\n  method: get\n  operationId: searchEpisodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search\n  method: options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /api/feed-index\n  method: get\n  operationId: getFeedIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/feed-index\n  method: options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/feed-index/person/{person}\n  method: get\n  operationId: getFeedIndexByPerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/feed-index/person/{person}\n  method: options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/feed-index/show/{show}\n  method: get\n  operationId: getFeedIndexByShow\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/feed-index/show/{show}\n  method: options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dl/{slug}/{file}\n  method: get\n  operationId: downloadEpisodeArtifact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dl/show/{show}/{file}\n  method: get\n  operationId: downloadShowArchive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/bidclub-ai/agentic-access/bidclub-ai-agentic-access.yml
summary_line: 22 operations · 4 acting
tags:
- Company
- Investment
- Podcasts
- Research
---

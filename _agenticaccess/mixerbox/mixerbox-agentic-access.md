---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 21
api_specs:
- filename: mixerbox-gpt-api-openapi.yml
  format: yaml
  label: MixerBox Gpt API
  slug: mixerbox-gpt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-gpt-api-openapi.yml
- filename: mixerbox-gpt-plugins-api-openapi.yml
  format: yaml
  label: MixerBox Gpt Plugins API
  slug: mixerbox-gpt-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-gpt-plugins-api-openapi.yml
- filename: mixerbox-services-api-openapi.yml
  format: yaml
  label: MixerBox Services API
  slug: mixerbox-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-services-api-openapi.yml
consequence_counts:
  read: 21
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mixerbox Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 29
overview: 'MixerBox exposes 29 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MixerBox
provider_slug: mixerbox
slug: mixerbox-agentic-access
source_filename: mixerbox-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/mixerbox-gpt-api-openapi.yml, openapi/mixerbox-gpt-plugins-api-openapi.yml,\n  openapi/mixerbox-services-funcs-getweatherinfo-mobile-0-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 21\n    acting: 8\n  by_consequence:\n    read: 21\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /gpt/getPlaylists\n  method: get\n  operationId: getPlaylistByType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpt/searchMusic\n  method: get\n  operationId: searchMusic\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpt/getPodcastsByCategory\n  method: get\n  operationId: getPodcastsByCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpt/searchPodcast\n  method: get\n  operationId: searchPodcast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpt/getPodcastsByCategoryMB\n  method: get\n  operationId: getPodcastsByCategoryInZhTw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpt/getPopularPodcasts\n  method: get\n  operationId: getPopularPodcasts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /gpt/getPopularEpisodes\n  method: get\n  operationId: getPopularEpisodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpt/getEpisodesByCategory\n  method: get\n  operationId: getEpisodesByCategoryInZhTw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpt/getEpisodesByPodcast\n  method: get\n  operationId: getEpisodesByPodcast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/calendar/authorize\n  method: get\n  operationId: Authorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/calendar/logout\n\
  \  method: get\n  operationId: Logout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/calendar/list\n  method: get\n  operationId: ListCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/calendar/events\n  method: get\n  operationId: ListEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/calendar/add_event\n  method: post\n  operationId: AddEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/gpt_plugins/calendar/free\n  method: get\n  operationId: GetFreeTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/chat_pdf/upload\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/gpt_plugins/chat_pdf/query\n  method: post\n  operationId: queryFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/diagrams/render\n  method: get\n  operationId: render\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/image_gen\n  method: get\n  operationId: imageGeneration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/photo_magic/super_resolution\n  method: get\n  operationId: EnhanceResolution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/prompt_pro/prompt_optimize\n  method: post\n  operationId: rephrase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/gpt_plugins/qr/generate\n  method: post\n  operationId: generateQr\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/gpt_plugins/scholar/upload\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/gpt_plugins/scholar/query\n  method: post\n  operationId: queryFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/scholar/abstract\n  method: post\n  operationId: searchAbstract\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/translate/translate\n  method: post\n  operationId: translate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/gpt_plugins/translate/explain\n  method: post\n  operationId: explain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/gpt_plugins/translate/task\n  method: post\n  operationId: task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services?funcs=GetWeatherInfo&mobile=0\n  method: get\n  operationId: getWeatherInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/agentic-access/mixerbox-agentic-access.yml
summary_line: 29 operations · 8 acting
tags:
- Company
- Consumer
- Artificial Intelligence
- ChatGPT Plugins
- GPT Actions
- Music
- Podcasts
- Weather
- Translation
- Productivity
---

---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 20
api_specs:
- filename: mixerbox-oneplayer-openapi-original.json
  format: json
  label: MixerBox OnePlayer
  slug: mixerbox-oneplayer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-oneplayer-openapi-original.json
- filename: mixerbox-podcasts-openapi-original.json
  format: json
  label: MixerBox Podcasts
  slug: mixerbox-podcasts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-podcasts-openapi-original.json
- filename: mixerbox-weather-openapi-original.json
  format: json
  label: MixerBox Weather
  slug: mixerbox-weather
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-weather-openapi-original.json
- filename: mixerbox-calendar-openapi-original.json
  format: json
  label: MixerBox Calendar
  slug: mixerbox-calendar
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-calendar-openapi-original.json
- filename: mixerbox-translate-openapi-original.json
  format: json
  label: MixerBox Translate
  slug: mixerbox-translate
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-translate-openapi-original.json
- filename: mixerbox-imagegen-openapi-original.json
  format: json
  label: MixerBox ImageGen
  slug: mixerbox-imagegen
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-imagegen-openapi-original.json
- filename: mixerbox-photomagic-openapi-original.json
  format: json
  label: MixerBox PhotoMagic
  slug: mixerbox-photomagic
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-photomagic-openapi-original.json
- filename: mixerbox-chatpdf-openapi-original.json
  format: json
  label: MixerBox ChatPDF
  slug: mixerbox-chatpdf
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-chatpdf-openapi-original.json
- filename: mixerbox-scholar-openapi-original.json
  format: json
  label: MixerBox Scholar
  slug: mixerbox-scholar
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-scholar-openapi-original.json
- filename: mixerbox-qr-openapi-original.json
  format: json
  label: MixerBox QR
  slug: mixerbox-qr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-qr-openapi-original.json
- filename: mixerbox-diagrams-openapi-original.json
  format: json
  label: MixerBox Diagrams
  slug: mixerbox-diagrams
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-diagrams-openapi-original.json
- filename: mixerbox-promptpro-openapi-original.json
  format: json
  label: MixerBox Prompt Pro
  slug: mixerbox-prompt-pro
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/openapi/mixerbox-promptpro-openapi-original.json
consequence_counts:
  read: 20
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mixerbox Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 31
overview: 'MixerBox exposes 31 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MixerBox
provider_slug: mixerbox
slug: mixerbox-agentic-access
source_filename: mixerbox-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/mixerbox-calendar-openapi-original.json, openapi/mixerbox-chatpdf-openapi-original.json,\n  openapi/mixerbox-diagrams-openapi-original.json, openapi/mixerbox-imagegen-openapi-original.json,\n  openapi/mixerbox-oneplayer-openapi-original.json, openapi/mixerbox-photomagic-openapi-original.json,\n  openapi/mixerbox-podcasts-openapi-original.json, openapi/mixerbox-promptpro-openapi-original.json,\n  openapi/mixerbox-qr-openapi-original.json, openapi/mixerbox-scholar-openapi-original.json,\n  openapi/mixerbox-translate-openapi-original.json, openapi/mixerbox-weather-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 20\n    acting:\
  \ 11\n  by_consequence:\n    read: 20\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /api/gpt_plugins/calendar/authorize\n  method: get\n  operationId: Authorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/calendar/logout\n  method: get\n  operationId: Logout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/calendar/list\n  method: get\n  operationId: ListCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/calendar/events\n  method: get\n  operationId: ListEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/gpt_plugins/calendar/add_event\n  method: post\n  operationId: AddEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/gpt_plugins/calendar/free\n  method: get\n  operationId: GetFreeTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/chat_pdf/upload\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/gpt_plugins/chat_pdf/query\n\
  \  method: post\n  operationId: queryFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/gpt_plugins/diagrams/render\n  method: get\n  operationId: render\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/image_gen\n  method: get\n  operationId: imageGeneration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpt/getPlaylists\n  method: get\n  operationId: getPlaylistByType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /gpt/searchMusic\n  method: get\n  operationId: searchMusic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpt/getPodcastsByCategory\n  method: get\n  operationId: getPodcastsByCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpt/searchPodcast\n  method: get\n  operationId: searchPodcast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/photo_magic/super_resolution\n  method: get\n  operationId: EnhanceResolution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpt/getPodcastsByCategoryMB\n  method: get\n  operationId: getPodcastsByCategoryInZhTw\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpt/getPodcastsByCategory\n  method: get\n  operationId: getPodcastsByCategoryGlobal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpt/searchPodcast\n  method: get\n  operationId: searchPodcast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpt/getPopularPodcasts\n  method: get\n  operationId: getPopularPodcasts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpt/getPopularEpisodes\n  method: get\n  operationId: getPopularEpisodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpt/getEpisodesByCategory\n  method: get\n  operationId: getEpisodesByCategoryInZhTw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpt/getEpisodesByPodcast\n  method: get\n  operationId: getEpisodesByPodcast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt_plugins/prompt_pro/prompt_optimize\n  method: post\n  operationId: rephrase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/gpt_plugins/qr/generate\n  method: post\n  operationId: generateQr\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/gpt_plugins/scholar/upload\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/gpt_plugins/scholar/query\n  method: post\n  operationId: queryFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/gpt_plugins/scholar/abstract\n\
  \  method: post\n  operationId: searchAbstract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/gpt_plugins/translate/translate\n  method: post\n  operationId: translate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/gpt_plugins/translate/explain\n  method: post\n  operationId: explain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /api/gpt_plugins/translate/task\n  method: post\n  operationId: task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services?funcs=GetWeatherInfo&mobile=0\n  method: get\n  operationId: getWeatherInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mixerbox/refs/heads/main/agentic-access/mixerbox-agentic-access.yml
summary_line: 31 operations · 11 acting
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

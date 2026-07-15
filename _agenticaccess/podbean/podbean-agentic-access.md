---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 10
api_specs:
- filename: podbean-openapi.yml
  format: yaml
  label: Podbean Podcasts API
  slug: podbean-podcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/openapi/podbean-openapi.yml
- filename: podbean-openapi.yml
  format: yaml
  label: Podbean Episodes API
  slug: podbean-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/openapi/podbean-openapi.yml
- filename: podbean-openapi.yml
  format: yaml
  label: Podbean Media Files API
  slug: podbean-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/openapi/podbean-openapi.yml
- filename: podbean-openapi.yml
  format: yaml
  label: Podbean Analytics API
  slug: podbean-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/openapi/podbean-openapi.yml
- filename: podbean-openapi.yml
  format: yaml
  label: Podbean oEmbed API
  slug: podbean-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/openapi/podbean-openapi.yml
consequence_counts:
  read: 10
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Podbean Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Podbean exposes 16 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Podbean
provider_slug: podbean
slug: podbean-agentic-access
source_filename: podbean-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/podbean-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 10\n    acting: 6\n  by_consequence:\n    read: 10\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /dialog/oauth\n  method: get\n  operationId: loginDialog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/token\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/debugToken\n  method: post\n  operationId: debugToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/multiplePodcastsToken\n  method: post\n  operationId: getMultiplePodcastsToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /podcast\n  method: get\n  operationId: getPodcast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /episodes\n  method: get\n  operationId: listEpisodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /episodes\n  method: post\n  operationId: publishEpisode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /episodes/{id}\n  method: get\n  operationId: getEpisode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /episodes/{id}\n  method: post\n  operationId: updateEpisode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /episodes/{id}/delete\n  method: post\n  operationId: deleteEpisode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/uploadAuthorize\n  method: get\n  operationId: authorizeFileUpload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /medias\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oembed\n  method: get\n  operationId: oembed\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/podcastReports\n  method: get\n  operationId: getPodcastDownloadReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/podcastEngagementReports\n  method: get\n  operationId: getPodcastEngagementReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/advertiseReports\n  method: get\n  operationId: getAdvertiseReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/agentic-access/podbean-agentic-access.yml
summary_line: 16 operations · 6 acting
tags:
- Podcasting
- Podcast Hosting
- Media
- Audio
- Episodes
- Analytics
- Monetization
---

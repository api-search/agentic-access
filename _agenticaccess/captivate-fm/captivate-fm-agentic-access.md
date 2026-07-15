---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 18
api_specs:
- filename: captivate-fm-openapi.yml
  format: yaml
  label: Captivate Users API
  slug: captivate-fm-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivate-fm/refs/heads/main/openapi/captivate-fm-openapi.yml
- filename: captivate-fm-openapi.yml
  format: yaml
  label: Captivate Shows API
  slug: captivate-fm-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivate-fm/refs/heads/main/openapi/captivate-fm-openapi.yml
- filename: captivate-fm-openapi.yml
  format: yaml
  label: Captivate Episodes API
  slug: captivate-fm-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivate-fm/refs/heads/main/openapi/captivate-fm-openapi.yml
- filename: captivate-fm-openapi.yml
  format: yaml
  label: Captivate Media API
  slug: captivate-fm-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivate-fm/refs/heads/main/openapi/captivate-fm-openapi.yml
- filename: captivate-fm-openapi.yml
  format: yaml
  label: Captivate Analytics API
  slug: captivate-fm-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivate-fm/refs/heads/main/openapi/captivate-fm-openapi.yml
consequence_counts:
  read: 18
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Captivate Fm Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'Captivate exposes 28 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Captivate
provider_slug: captivate-fm
slug: captivate-fm-agentic-access
source_filename: captivate-fm-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/captivate-fm-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    acting: 10\n    connected: 18\n  by_consequence:\n    write: 10\n    read: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /authenticate/token\n  method: post\n  operationId: authenticateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}/shows\n  method: get\n  operationId: getUserShows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}/shows/manager\n  method: get\n  operationId: getUserManagedShows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shows/{id}/\n  method: get\n  operationId: getShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shows/{id}\n  method: put\n  operationId: updateShow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shows/{id}/artwork\n  method: post\n  operationId: createShowArtwork\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shows/{id}/feed\n  method: get\n  operationId: getShowFeedUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shows/{id}/episodes\n  method: get\n  operationId: getShowEpisodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shows/{id}/episodes/scheduled\n  method: get\n  operationId: getShowScheduledEpisodes\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /episodes/{id}\n  method: get\n  operationId: getEpisode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /episodes/{id}\n  method: put\n  operationId: updateEpisode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /episodes\n  method: post\n  operationId: createEpisode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /media/{id}\n  method: get\n  operationId: getMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shows/{id}/media\n  method: post\n  operationId: uploadMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shows/{id}/media\n  method: get\n  operationId: getShowMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shows/{id}/media/search\n  method: get\n  operationId: searchShowMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /insights/{showId}/overview\n  method: get\n  operationId: getPodcastOverviewAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/{showId}/overview/{episodeId}\n  method: get\n  operationId: getEpisodeOverviewAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/{showId}/averages\n  method: get\n  operationId: getPodcastAverageAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/{showId}/total\n  method: get\n  operationId: getPodcastAllTimeTotal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/{showId}/total/{episodeId}\n\
  \  method: get\n  operationId: getEpisodeAllTimeTotal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/{showId}/monthly\n  method: get\n  operationId: getPodcastMonthlyAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/{showId}/monthly/{episodeId}\n  method: get\n  operationId: getEpisodeMonthlyAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/{showId}/range\n  method: post\n  operationId: getPodcastRangeAnalytics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /insights/{showId}/range/{episodeId}\n  method: post\n  operationId: getEpisodeRangeAnalytics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/{showId}/compare\n  method: post\n  operationId: compareEpisodeAnalytics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/{showId}/web-player/{episodeId}\n  method: post\n  operationId: getWebPlayerAnalytics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/captivate-fm/refs/heads/main/agentic-access/captivate-fm-agentic-access.yml
summary_line: 28 operations · 10 acting
tags:
- Podcasting
- Podcast Hosting
- Episodes
- Media
- Analytics
- RSS
---

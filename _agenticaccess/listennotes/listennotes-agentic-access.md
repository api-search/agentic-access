---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 21
api_specs:
- filename: listennotes-directory-api-api-openapi.yml
  format: yaml
  label: Listen Notes Directory API API
  slug: listennotes-directory-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-directory-api-api-openapi.yml
- filename: listennotes-insights-api-api-openapi.yml
  format: yaml
  label: Listen Notes Insights API API
  slug: listennotes-insights-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-insights-api-api-openapi.yml
- filename: listennotes-playlist-api-api-openapi.yml
  format: yaml
  label: Listen Notes Playlist API API
  slug: listennotes-playlist-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-playlist-api-api-openapi.yml
- filename: listennotes-podcaster-api-api-openapi.yml
  format: yaml
  label: Listen Notes Podcaster API API
  slug: listennotes-podcaster-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-podcaster-api-api-openapi.yml
- filename: listennotes-search-api-api-openapi.yml
  format: yaml
  label: Listen Notes Search API API
  slug: listennotes-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/openapi/listennotes-search-api-api-openapi.yml
consequence_counts:
  read: 21
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Listennotes Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Listen Notes exposes 26 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Listen Notes
provider_slug: listennotes
slug: listennotes-agentic-access
source_filename: listennotes-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/listennotes-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 21\n    acting: 5\n  by_consequence:\n    read: 21\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /typeahead\n  method: get\n  operationId: typeahead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search_episode_titles\n  method: get\n  operationId:\
  \ searchEpisodeTitles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trending_searches\n  method: get\n  operationId: trendingSearches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /related_searches\n  method: get\n  operationId: relatedSearches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spellcheck\n  method: get\n  operationId: spellcheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /best_podcasts\n  method: get\n  operationId: bestPodcasts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /podcasts/{id}\n  method: get\n  operationId: getPodcastById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /podcasts/{id}\n  method: delete\n  operationId: deletePodcastById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /episodes/{id}\n  method: get\n  operationId: getEpisodeById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /episodes\n  method: post\n  operationId: batchGetEpisodes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /podcasts\n  method: post\n  operationId: batchGetPodcasts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /curated_podcasts\n  method: get\n  operationId: getCuratedPodcasts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /curated_podcasts/{id}\n  method: get\n  operationId: getCuratedPodcastById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /genres\n  method: get\n  operationId:\
  \ getGenres\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regions\n  method: get\n  operationId: getRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /languages\n  method: get\n  operationId: getLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /just_listen\n  method: get\n  operationId: justListen\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /podcasts/{id}/recommendations\n  method: get\n  operationId: getPodcastRecommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /episodes/{id}/recommendations\n  method: get\n  operationId: getEpisodeRecommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /playlists\n  method: get\n  operationId: getPlaylists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /playlists/{id}\n  method: get\n  operationId: getPlaylistById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /podcasts/{id}/audience\n  method: get\n  operationId: getPodcastAudience\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /podcasts/domains/{domain_name}\n  method: get\n  operationId: getPodcastsByDomain\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /podcasts/submit\n  method: post\n  operationId: submitPodcast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /podcasts/{id}/rss\n  method: post\n  operationId: refreshPodcastRss\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listennotes/refs/heads/main/agentic-access/listennotes-agentic-access.yml
summary_line: 26 operations · 5 acting
tags:
- Podcasts
- Podcast Search
- Podcast Directory
- Search
- Audio
- Media
- Podcast Insights
---

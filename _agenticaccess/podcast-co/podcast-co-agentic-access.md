---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: podcast-co-episodes-api-openapi.yml
  format: yaml
  label: Podcast.co Episodes API
  slug: podcast-co-episodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/podcast-co/openapi/podcast-co-episodes-api-openapi.yml
- filename: podcast-co-podcast-page-api-openapi.yml
  format: yaml
  label: Podcast.co podcast page API
  slug: podcast-co-podcast-page-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/podcast-co/openapi/podcast-co-podcast-page-api-openapi.yml
- filename: podcast-co-podcasts-api-openapi.yml
  format: yaml
  label: Podcast.co Podcasts API
  slug: podcast-co-podcasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/podcast-co/openapi/podcast-co-podcasts-api-openapi.yml
- filename: podcast-co-subscribe-button-api-openapi.yml
  format: yaml
  label: Podcast.co subscribe button API
  slug: podcast-co-subscribe-button-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/podcast-co/openapi/podcast-co-subscribe-button-api-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Podcast Co Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Podcast.co exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Podcast.co
provider_slug: podcast-co
slug: podcast-co-agentic-access
source_filename: podcast-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/podcast-co-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /podcasts/{podcast_slug}\n  method: get\n  operationId: getPodcast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /podcasts/{podcast_slug}/player\n  method: get\n  operationId: getPodcastPlayer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /podcasts/{podcast_slug}/subscribe_button\n\
  \  method: get\n  operationId: getPodcastSubscribeButton\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /podcasts/{podcast_slug}/socials\n  method: get\n  operationId: getPodcastSocials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /podcasts/{podcast_slug}/directories\n  method: get\n  operationId: getPodcastDirectories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /podcasts/{podcast_slug}/donations\n  method: get\n  operationId: getPodcastDonations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /podcasts/{podcast_slug}/page\n  method: get\n  operationId: getPodcastPageSettings\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /podcasts/{podcast_slug}/hosts\n  method: get\n  operationId: listPodcastHosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /podcasts/{podcast_slug}/episodes\n  method: get\n  operationId: listPodcastsEpisodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /podcasts/{podcast_slug}/episodes/{episode_slug}\n  method: get\n  operationId: getEpisode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /podcasts/{podcast_slug}/episodes/{episode_slug}/player\n  method: get\n  operationId: getEpisodePlayer\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/podcast-co/agentic-access/podcast-co-agentic-access.yml
summary_line: 11 operations
tags:
- Podcasts
- Hosting
- Audio
- Software-as-a-Service
- Media
---

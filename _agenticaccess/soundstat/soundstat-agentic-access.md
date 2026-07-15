---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 5
api_specs:
- filename: soundstat-openapi.yml
  format: yaml
  label: SoundStat Track Analysis API
  slug: soundstat-track-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundstat/refs/heads/main/openapi/soundstat-openapi.yml
- filename: soundstat-openapi.yml
  format: yaml
  label: SoundStat Search & Discovery API
  slug: soundstat-search-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundstat/refs/heads/main/openapi/soundstat-openapi.yml
- filename: soundstat-openapi.yml
  format: yaml
  label: SoundStat Recommendations API
  slug: soundstat-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundstat/refs/heads/main/openapi/soundstat-openapi.yml
consequence_counts:
  read: 5
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Soundstat Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'SoundStat exposes 20 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SoundStat
provider_slug: soundstat
slug: soundstat-agentic-access
source_filename: soundstat-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/soundstat-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 5\n    acting: 15\n  by_consequence:\n    read: 5\n    write: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/track/{track_id}\n  method: get\n  operationId: get_track_analysis_api_v1_track__track_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/track/{track_id}/status\n  method: get\n  operationId: track_status_updates_api_v1_track__track_id__status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tracks/search\n  method: post\n  operationId: search_tracks_api_v1_tracks_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/genres\n  method: get\n  operationId: get_available_genres_api_v1_genres_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/recommendations/similar\n  method: get\n  operationId: get_similar_tracks_api_v1_recommendations_similar_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/recommendations/by-features\n\
  \  method: post\n  operationId: get_recommendations_by_features_api_v1_recommendations_by_features_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recommendations/mixed\n  method: post\n  operationId: get_mixed_recommendations_api_v1_recommendations_mixed_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/stats\n  method: get\n  operationId: get_analysis_stats_api_v1_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/recommendations/progression\n  method: post\n  operationId: get_progression_recommendations_api_v1_recommendations_progression_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recommendations/compatible\n  method: post\n  operationId: get_compatible_tracks_api_v1_recommendations_compatible_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recommendations/contrast\n  method: post\n  operationId: get_contrast_recommendations_api_v1_recommendations_contrast_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recommendations/cross-genre\n  method: post\n  operationId: get_cross_genre_recommendations_api_v1_recommendations_cross_genre_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recommendations/time-of-day\n  method: post\n  operationId: get_time_of_day_recommendations_api_v1_recommendations_time_of_day_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recommendations/hidden-gems\n  method: post\n  operationId: get_hidden_gems_recommendations_api_v1_recommendations_hidden_gems_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recommendations/beat-structure\n  method: post\n  operationId: get_beat_structure_recommendations_api_v1_recommendations_beat_structure_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/v1/recommendations/duration\n  method: post\n  operationId: get_duration_recommendations_api_v1_recommendations_duration_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recommendations/mood\n  method: post\n  operationId: get_mood_recommendations_api_v1_recommendations_mood_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recommendations/activity\n  method: post\n  operationId: get_activity_recommendations_api_v1_recommendations_activity_post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recommendations/instrumental\n  method: post\n  operationId: get_instrumental_recommendations_api_v1_recommendations_instrumental_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recommendations/acoustic\n  method: post\n  operationId: get_acoustic_recommendations_api_v1_recommendations_acoustic_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soundstat/refs/heads/main/agentic-access/soundstat-agentic-access.yml
summary_line: 20 operations · 15 acting
tags:
- Music
- Audio Analysis
- Audio Features
- Recommendations
- Track Analysis
- Spotify Alternative
---

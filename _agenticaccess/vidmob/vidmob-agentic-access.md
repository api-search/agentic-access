---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 8
api_specs:
- filename: vidmob-media-api-openapi.yml
  format: yaml
  label: VidMob Media API
  slug: vidmob-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/openapi/vidmob-media-api-openapi.yml
- filename: vidmob-organization-api-openapi.yml
  format: yaml
  label: VidMob Organization API
  slug: vidmob-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/openapi/vidmob-organization-api-openapi.yml
- filename: vidmob-scoring-api-openapi.yml
  format: yaml
  label: VidMob Scoring API
  slug: vidmob-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/openapi/vidmob-scoring-api-openapi.yml
- filename: vidmob-workspaces-api-openapi.yml
  format: yaml
  label: VidMob Workspaces API
  slug: vidmob-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/openapi/vidmob-workspaces-api-openapi.yml
consequence_counts:
  read: 8
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vidmob Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'VidMob exposes 11 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: VidMob
provider_slug: vidmob
slug: vidmob-agentic-access
source_filename: vidmob-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: generated\nsource: openapi/vidmob-creative-aperture-openapi.json, openapi/vidmob-creative-scoring-openapi.json,\n  openapi/vidmob-public-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 8\n    acting: 3\n  by_consequence:\n    read: 8\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/media/aperture/{jobId}\n  method: get\n  operationId: get-creative-aperture-job-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/media/aperture\n  method: post\n  operationId: create-creative-aperture-job\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scoring/workspace/{workspaceId}/scorecards\n  method: get\n  operationId: get-workspace-scorecards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scoring/media/{mediaId}/scores\n  method: get\n  operationId: get-media-score\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/media\n  method: post\n  operationId: upload-media-for-scoring\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/media/{mediaId}/status\n  method: get\n  operationId: get-media-scoring-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scoring/criteria/metadata\n  method: post\n  operationId: get-criteria-metadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scoring/scorecard/{scorecardId}/media-metadata\n  method: get\n  operationId: get_v1scoringworkspace{workspaceId}scorecards-1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/media/updated-scores\n\
  \  method: get\n  operationId: get_v1mediaupdated-scores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organization\n  method: get\n  operationId: get-organization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces\n  method: get\n  operationId: get-organization-copy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/agentic-access/vidmob-agentic-access.yml
summary_line: 11 operations · 3 acting
tags:
- Creative Intelligence
- creative-data
- Advertising
- Marketing
- Media Measurement
- Video
- Computer-Vision
- Creative Analytics
- AdTech
- MCP
- agent-native
- MarTech
---

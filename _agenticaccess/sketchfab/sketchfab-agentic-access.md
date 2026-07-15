---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 3
api_specs:
- filename: sketchfab-data-api-openapi.yml
  format: yaml
  label: Sketchfab Data API
  slug: sketchfab-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-data-api-openapi.yml
- filename: sketchfab-download-api-openapi.yml
  format: yaml
  label: Sketchfab Download API
  slug: sketchfab-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-download-api-openapi.yml
- filename: sketchfab-oembed-api-openapi.yml
  format: yaml
  label: Sketchfab oEmbed API
  slug: sketchfab-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-oembed-api-openapi.yml
- filename: sketchfab-oauth-api-openapi.yml
  format: yaml
  label: Sketchfab OAuth 2.0 API
  slug: sketchfab-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/openapi/sketchfab-oauth-api-openapi.yml
consequence_counts:
  read: 3
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sketchfab Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Sketchfab exposes 4 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sketchfab
provider_slug: sketchfab
slug: sketchfab-agentic-access
source_filename: sketchfab-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sketchfab-download-api-openapi.yml, openapi/sketchfab-oauth-api-openapi.yml,\n  openapi/sketchfab-oembed-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 3\n    acting: 1\n  by_consequence:\n    read: 3\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/models/{uid}/download\n  method: get\n  operationId: getModelDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth2/authorize/\n  method: get\n  operationId: oauthAuthorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth2/token/\n  method: post\n  operationId: oauthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oembed\n  method: get\n  operationId: getOEmbed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/agentic-access/sketchfab-agentic-access.yml
summary_line: 4 operations · 1 acting
tags:
- 3D
- Models
- Marketplace
- Viewer
- WebGL
- glTF
- AR
- VR
- Creative
- Epic Games
---

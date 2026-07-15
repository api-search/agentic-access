---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 9
api_specs:
- filename: swagger
  format: yaml
  label: Getty Images API
  slug: platform
  spec_type: OpenAPI
  url: https://api.gettyimages.com/swagger
consequence_counts:
  read: 9
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Getty Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Getty Images exposes 10 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Getty Images
provider_slug: getty
slug: getty-agentic-access
source_filename: getty-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/getty-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 9\n    acting: 1\n  by_consequence:\n    read: 9\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /search/images/creative\n  method: get\n  operationId: searchImagesCreative\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - download\n    - read\n- path: /search/images/editorial\n  method: get\n  operationId: searchImagesEditorial\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n    scope:\n    - download\n    - read\n- path: /search/videos/creative\n  method: get\n  operationId: searchVideosCreative\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - download\n    - read\n- path: /search/videos/editorial\n  method: get\n  operationId: searchVideosEditorial\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - download\n    - read\n- path: /images\n  method: get\n  operationId: getImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - download\n    - read\n- path: /images/{id}\n  method: get\n  operationId: getImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - download\n    - read\n- path: /videos\n  method: get\n  operationId: getVideos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - download\n    - read\n- path: /videos/{id}\n  method: get\n  operationId: getVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - download\n    - read\n- path: /downloads/{image_id}\n  method: post\n  operationId: downloadImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - download\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /countries\n  method:\
  \ get\n  operationId: getCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - download\n    - read\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getty/refs/heads/main/agentic-access/getty-agentic-access.yml
summary_line: 10 operations · 1 acting
tags:
- Stock Media
- Images
- Editorial
- Video
- Music
- Licensing
---

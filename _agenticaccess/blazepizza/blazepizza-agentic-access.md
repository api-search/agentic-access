---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 5
api_specs:
- filename: blazepizza-blazepizza-api-api-openapi.yml
  format: yaml
  label: Blazepizza Blazepizza API
  slug: blazepizza-blazepizza-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazepizza/openapi/blazepizza-blazepizza-api-api-openapi.yml
- filename: blazepizza-cat-pic-api-openapi.yml
  format: yaml
  label: Blazepizza Cat Pic API
  slug: blazepizza-cat-pic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazepizza/openapi/blazepizza-cat-pic-api-openapi.yml
- filename: blazepizza-foo-api-openapi.yml
  format: yaml
  label: Blazepizza Foo API
  slug: blazepizza-foo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazepizza/openapi/blazepizza-foo-api-openapi.yml
- filename: blazepizza-http-api-openapi.yml
  format: yaml
  label: Blazepizza HTTP API
  slug: blazepizza-http-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazepizza/openapi/blazepizza-http-api-openapi.yml
- filename: blazepizza-image-api-openapi.yml
  format: yaml
  label: Blazepizza Image API
  slug: blazepizza-image-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazepizza/openapi/blazepizza-image-api-openapi.yml
consequence_counts:
  read: 5
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Blazepizza Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Blazepizza exposes 7 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Blazepizza
provider_slug: blazepizza
slug: blazepizza-agentic-access
source_filename: blazepizza-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/blazepizza-blazepizza-api-api-openapi.yml, openapi/blazepizza-cat-pic-api-openapi.yml,\n  openapi/blazepizza-foo-api-openapi.yml, openapi/blazepizza-http-api-openapi.yml, openapi/blazepizza-image-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 5\n    acting: 2\n  by_consequence:\n    read: 5\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: put\n  operationId: put\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cat-pic.jpg\n  method: get\n  operationId: get_cat_pic_jpg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cat-pic.jpg\n  method: put\n  operationId: put_cat_pic_jpg\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /foo\n  method: get\n  operationId: get_foo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /http/post/binary\n\
  \  method: get\n  operationId: get_http_post_binary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /image.png\n  method: get\n  operationId: get_image_png\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/blazepizza/agentic-access/blazepizza-agentic-access.yml
summary_line: 7 operations · 2 acting
tags:
- Company
- Fast Casual
- Pizza
- Restaurant
- Franchise
---

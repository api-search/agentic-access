---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 9
api_specs:
- filename: gumgum-image-api-openapi.yml
  format: yaml
  label: GumGum Image API
  slug: gumgum-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumgum/refs/heads/main/openapi/gumgum-image-api-openapi.yml
- filename: gumgum-intravideo-api-openapi.yml
  format: yaml
  label: GumGum Intravideo API
  slug: gumgum-intravideo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumgum/refs/heads/main/openapi/gumgum-intravideo-api-openapi.yml
- filename: gumgum-page-api-openapi.yml
  format: yaml
  label: GumGum Page API
  slug: gumgum-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumgum/refs/heads/main/openapi/gumgum-page-api-openapi.yml
- filename: gumgum-text-api-openapi.yml
  format: yaml
  label: GumGum Text API
  slug: gumgum-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumgum/refs/heads/main/openapi/gumgum-text-api-openapi.yml
- filename: gumgum-video-api-openapi.yml
  format: yaml
  label: GumGum Video API
  slug: gumgum-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumgum/refs/heads/main/openapi/gumgum-video-api-openapi.yml
consequence_counts:
  read: 9
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gumgum Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'GumGum exposes 13 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GumGum
provider_slug: gumgum
slug: gumgum-agentic-access
source_filename: gumgum-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: generated\nsource: openapi/gumgum-contextual-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 9\n    acting: 4\n  by_consequence:\n    read: 9\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /page/classify\n  method: get\n  operationId: classifyPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /video/classification\n  method: post\n  operationId: submitVideoClassification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video/classification/{uuid}\n  method: get\n  operationId: getVideoClassification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /video/classification/{uuid}/status\n  method: get\n  operationId: getVideoClassificationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/video/classification\n  method: post\n  operationId: submitIntravideoClassification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/video/classification/{uuid}\n\
  \  method: get\n  operationId: getIntravideoClassification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/video/classification/{uuid}/status\n  method: get\n  operationId: getIntravideoClassificationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /image/classification\n  method: post\n  operationId: submitImageClassification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /image/classification/{uuid}\n  method: get\n  operationId: getImageClassification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /image/classification/{uuid}/status\n  method: get\n  operationId: getImageClassificationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /text/classification\n  method: post\n  operationId: submitTextClassification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /text/classification/{uuid}\n  method: get\n  operationId: getTextClassification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /text/classification/{uuid}/status\n  method: get\n  operationId: getTextClassificationStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gumgum/refs/heads/main/agentic-access/gumgum-agentic-access.yml
summary_line: 13 operations · 4 acting
tags:
- Advertising
- adtech
- contextual-advertising
- brand-safety
- content-classification
- computer-vision
- natural-language-processing
- video-analysis
- image-analysis
- connected-tv
- header-bidding
- programmatic-advertising
- iab-taxonomy
- content-moderation
---

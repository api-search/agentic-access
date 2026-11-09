---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 6
api_specs:
- filename: asternym-com-bazi-api-openapi.yml
  format: yaml
  label: AsterNym Bazi API
  slug: asternym-com-bazi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asternym-com/openapi/asternym-com-bazi-api-openapi.yml
- filename: asternym-com-natal-api-openapi.yml
  format: yaml
  label: AsterNym Natal API
  slug: asternym-com-natal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asternym-com/openapi/asternym-com-natal-api-openapi.yml
- filename: asternym-com-numerology-api-openapi.yml
  format: yaml
  label: AsterNym Numerology API
  slug: asternym-com-numerology-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asternym-com/openapi/asternym-com-numerology-api-openapi.yml
- filename: asternym-com-reading-api-openapi.yml
  format: yaml
  label: AsterNym Reading API
  slug: asternym-com-reading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asternym-com/openapi/asternym-com-reading-api-openapi.yml
- filename: asternym-com-zodiac-api-openapi.yml
  format: yaml
  label: AsterNym Zodiac API
  slug: asternym-com-zodiac-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asternym-com/openapi/asternym-com-zodiac-api-openapi.yml
consequence_counts:
  read: 6
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Asternym Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'AsterNym exposes 12 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AsterNym
provider_slug: asternym-com
slug: asternym-com-agentic-access
source_filename: asternym-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/asternym-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 6\n    acting: 6\n  by_consequence:\n    read: 6\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/reading\n  method: get\n  operationId: getReading\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reading\n  method: post\n  operationId: postReading\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bazi\n  method: get\n  operationId: getBazi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bazi\n  method: post\n  operationId: postBazi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bazi/hours\n  method: get\n  operationId: getBaziHours\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bazi/hours\n  method: post\n  operationId: postBaziHours\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/numerology\n  method: get\n  operationId: getNumerology\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/numerology\n  method: post\n  operationId: postNumerology\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/zodiac\n  method: get\n  operationId: getZodiac\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/zodiac\n\
  \  method: post\n  operationId: postZodiac\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/natal\n  method: get\n  operationId: getNatal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/natal\n  method: post\n  operationId: postNatal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/asternym-com/agentic-access/asternym-com-agentic-access.yml
summary_line: 12 operations · 6 acting
tags:
- Astrology
- BaZi
- Numerology
- Compatibility
- BirthChart
---

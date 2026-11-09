---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 8
api_specs:
- filename: debriefing-io-openapi.json
  format: json
  label: Debriefing Read API
  slug: debriefing-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debriefing-io/openapi/debriefing-io-openapi.json
- filename: debriefing-io-battlecards-api-openapi.yml
  format: yaml
  label: Debriefing Battlecards API
  slug: debriefing-io-battlecards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debriefing-io/openapi/debriefing-io-battlecards-api-openapi.yml
- filename: debriefing-io-competitors-api-openapi.yml
  format: yaml
  label: Debriefing Competitors API
  slug: debriefing-io-competitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debriefing-io/openapi/debriefing-io-competitors-api-openapi.yml
- filename: debriefing-io-digests-api-openapi.yml
  format: yaml
  label: Debriefing Digests API
  slug: debriefing-io-digests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debriefing-io/openapi/debriefing-io-digests-api-openapi.yml
- filename: debriefing-io-signals-api-openapi.yml
  format: yaml
  label: Debriefing Signals API
  slug: debriefing-io-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debriefing-io/openapi/debriefing-io-signals-api-openapi.yml
consequence_counts:
  read: 8
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Debriefing Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Debriefing exposes 9 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Debriefing
provider_slug: debriefing-io
slug: debriefing-io-agentic-access
source_filename: debriefing-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/debriefing-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 8\n    acting: 1\n  by_consequence:\n    read: 8\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/competitors\n  method: get\n  operationId: listCompetitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/competitors\n  method: post\n  operationId: addCompetitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - watchlist:add\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/competitors/{id}\n  method: get\n  operationId: getCompetitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signals\n  method: get\n  operationId: listSignals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signals/{id}\n  method: get\n  operationId: getSignal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/digests\n  method: get\n  operationId: listDigests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/digests/{id}\n  method: get\n  operationId: getDigest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/battlecards\n  method: get\n  operationId: listBattlecards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/battlecards/{id}\n  method: get\n  operationId: getBattlecard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/debriefing-io/agentic-access/debriefing-io-agentic-access.yml
summary_line: 9 operations · 1 acting
tags:
- Competitive Intelligence
- Software-as-a-Service
- B2B
- Monitoring
- Small Business
---

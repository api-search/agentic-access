---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 26
api_specs:
- filename: ceramic-config-api-openapi.yml
  format: yaml
  label: Ceramic Config API
  slug: ceramic-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-config-api-openapi.yml
- filename: ceramic-debug-api-openapi.yml
  format: yaml
  label: Ceramic Debug API
  slug: ceramic-debug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-debug-api-openapi.yml
- filename: ceramic-events-api-openapi.yml
  format: yaml
  label: Ceramic Events API
  slug: ceramic-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-events-api-openapi.yml
- filename: ceramic-experimental-api-openapi.yml
  format: yaml
  label: Ceramic Experimental API
  slug: ceramic-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-experimental-api-openapi.yml
- filename: ceramic-feed-api-openapi.yml
  format: yaml
  label: Ceramic Feed API
  slug: ceramic-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-feed-api-openapi.yml
- filename: ceramic-interests-api-openapi.yml
  format: yaml
  label: Ceramic Interests API
  slug: ceramic-interests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-interests-api-openapi.yml
- filename: ceramic-liveness-api-openapi.yml
  format: yaml
  label: Ceramic Liveness API
  slug: ceramic-liveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-liveness-api-openapi.yml
- filename: ceramic-peers-api-openapi.yml
  format: yaml
  label: Ceramic Peers API
  slug: ceramic-peers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-peers-api-openapi.yml
- filename: ceramic-streams-api-openapi.yml
  format: yaml
  label: Ceramic Streams API
  slug: ceramic-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-streams-api-openapi.yml
- filename: ceramic-version-api-openapi.yml
  format: yaml
  label: Ceramic Version API
  slug: ceramic-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-version-api-openapi.yml
consequence_counts:
  read: 26
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ceramic Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'Ceramic exposes 30 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ceramic
provider_slug: ceramic
slug: ceramic-agentic-access
source_filename: ceramic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/ceramic-config-api-openapi.yml, openapi/ceramic-debug-api-openapi.yml, openapi/ceramic-events-api-openapi.yml,\n  openapi/ceramic-experimental-api-openapi.yml, openapi/ceramic-feed-api-openapi.yml, openapi/ceramic-interests-api-openapi.yml,\n  openapi/ceramic-liveness-api-openapi.yml, openapi/ceramic-peers-api-openapi.yml, openapi/ceramic-streams-api-openapi.yml,\n  openapi/ceramic-version-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 26\n    acting: 4\n  by_consequence:\n    read: 26\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /config/network\n  method: options\n  operationId: optionsConfigNetwork\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/network\n  method: get\n  operationId: getConfigNetwork\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /debug/heap\n  method: options\n  operationId: optionsDebugHeap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /debug/heap\n  method: get\n  operationId: getDebugHeap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: options\n  operationId: optionsEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /events\n  method: post\n  operationId: postEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{event_id}\n  method: options\n  operationId: optionsEventsByEventId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{event_id}\n  method: get\n  operationId: getEventsByEventId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /experimental/interests\n  method: options\n  operationId: optionsExperimentalInterests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /experimental/interests\n  method: get\n  operationId: getExperimentalInterests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /experimental/events/{sep}/{sepValue}\n  method: options\n  operationId: optionsExperimentalEventsBySepBySepValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /experimental/events/{sep}/{sepValue}\n  method: get\n  operationId: getExperimentalEventsBySepBySepValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feed/events\n  method: options\n  operationId: optionsFeedEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /feed/events\n  method: get\n  operationId: getFeedEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feed/resumeToken\n  method: options\n  operationId: optionsFeedResumeToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feed/resumeToken\n  method: get\n  operationId: getFeedResumeToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /interests/{sort_key}/{sort_value}\n  method: options\n  operationId: optionsInterestsBySortKeyBySortValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /interests/{sort_key}/{sort_value}\n \
  \ method: post\n  operationId: postInterestsBySortKeyBySortValue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /interests\n  method: options\n  operationId: optionsInterests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /interests\n  method: post\n  operationId: postInterests\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /liveness\n  method: options\n  operationId: optionsLiveness\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /liveness\n  method: get\n  operationId: getLiveness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /peers\n  method: options\n  operationId: optionsPeers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /peers\n  method: get\n  operationId: getPeers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /peers\n  method: post\n  operationId: postPeers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /streams/{stream_id}\n  method: options\n  operationId: optionsStreamsByStreamId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /streams/{stream_id}\n  method: get\n  operationId: getStreamsByStreamId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /version\n  method: options\n  operationId: optionsVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /version\n  method: get\n  operationId: getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /version\n  method: post\n  operationId: postVersion\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/agentic-access/ceramic-agentic-access.yml
summary_line: 30 operations · 4 acting
tags:
- Decentralized
- Web3
- Data Streams
- DID
- IPFS
- Blockchain
- Event Streaming
- ComposeDB
---

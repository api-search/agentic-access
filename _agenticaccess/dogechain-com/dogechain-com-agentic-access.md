---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: dogechain-com-address-api-openapi.yml
  format: yaml
  label: Dogechain Address API
  slug: dogechain-com-address-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dogechain-com/openapi/dogechain-com-address-api-openapi.yml
- filename: dogechain-com-block-api-openapi.yml
  format: yaml
  label: Dogechain Block API
  slug: dogechain-com-block-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dogechain-com/openapi/dogechain-com-block-api-openapi.yml
- filename: dogechain-com-blocks-api-openapi.yml
  format: yaml
  label: Dogechain Blocks API
  slug: dogechain-com-blocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dogechain-com/openapi/dogechain-com-blocks-api-openapi.yml
- filename: dogechain-com-chart-api-openapi.yml
  format: yaml
  label: Dogechain Chart API
  slug: dogechain-com-chart-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dogechain-com/openapi/dogechain-com-chart-api-openapi.yml
- filename: dogechain-com-fees-api-openapi.yml
  format: yaml
  label: Dogechain Fees API
  slug: dogechain-com-fees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dogechain-com/openapi/dogechain-com-fees-api-openapi.yml
- filename: dogechain-com-find-api-openapi.yml
  format: yaml
  label: Dogechain Find API
  slug: dogechain-com-find-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dogechain-com/openapi/dogechain-com-find-api-openapi.yml
- filename: dogechain-com-labels-api-openapi.yml
  format: yaml
  label: Dogechain Labels API
  slug: dogechain-com-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dogechain-com/openapi/dogechain-com-labels-api-openapi.yml
- filename: dogechain-com-live-api-openapi.yml
  format: yaml
  label: Dogechain Live API
  slug: dogechain-com-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dogechain-com/openapi/dogechain-com-live-api-openapi.yml
- filename: dogechain-com-network-api-openapi.yml
  format: yaml
  label: Dogechain Network API
  slug: dogechain-com-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dogechain-com/openapi/dogechain-com-network-api-openapi.yml
- filename: dogechain-com-richlist-api-openapi.yml
  format: yaml
  label: Dogechain Richlist API
  slug: dogechain-com-richlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dogechain-com/openapi/dogechain-com-richlist-api-openapi.yml
- filename: dogechain-com-supply-api-openapi.yml
  format: yaml
  label: Dogechain Supply API
  slug: dogechain-com-supply-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dogechain-com/openapi/dogechain-com-supply-api-openapi.yml
- filename: dogechain-com-tx-api-openapi.yml
  format: yaml
  label: Dogechain Tx API
  slug: dogechain-com-tx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dogechain-com/openapi/dogechain-com-tx-api-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dogechain Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Dogechain exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dogechain
provider_slug: dogechain-com
slug: dogechain-com-agentic-access
source_filename: dogechain-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/dogechain-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /address/{address}\n  method: get\n  operationId: getAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /block/{id}\n  method: get\n  operationId: getBlock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blocks/latest\n  method: get\n  operationId: getLatestBlocks\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chart/{series}\n  method: get\n  operationId: getChart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fees\n  method: get\n  operationId: getFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /find\n  method: get\n  operationId: find\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labels\n  method: get\n  operationId: getLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /live\n  method: get\n  operationId:\
  \ streamLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network\n  method: get\n  operationId: getNetwork\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /richlist\n  method: get\n  operationId: getRichList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /supply\n  method: get\n  operationId: getSupply\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tx/{txid}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dogechain-com/agentic-access/dogechain-com-agentic-access.yml
summary_line: 12 operations
tags:
- Blockchain
- Explorer
- Dogecoin
- Cryptocurrency
---

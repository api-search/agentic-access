---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 11
api_specs:
- filename: blazephoenix-xyz-abi-api-openapi.yml
  format: yaml
  label: BlazePhoenix Abi API
  slug: blazephoenix-xyz-abi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazephoenix-xyz/openapi/blazephoenix-xyz-abi-api-openapi.yml
- filename: blazephoenix-xyz-badge-api-openapi.yml
  format: yaml
  label: BlazePhoenix Badge API
  slug: blazephoenix-xyz-badge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazephoenix-xyz/openapi/blazephoenix-xyz-badge-api-openapi.yml
- filename: blazephoenix-xyz-blazephoenix-integration-api-your-rpc-api-openapi.yml
  format: yaml
  label: BlazePhoenix BlazePhoenix Integration API (your RPC) API
  slug: blazephoenix-xyz-blazephoenix-integration-api-your-rpc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazephoenix-xyz/openapi/blazephoenix-xyz-blazephoenix-integration-api-your-rpc-api-openapi.yml
- filename: blazephoenix-xyz-deployments-api-openapi.yml
  format: yaml
  label: BlazePhoenix Deployments API
  slug: blazephoenix-xyz-deployments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazephoenix-xyz/openapi/blazephoenix-xyz-deployments-api-openapi.yml
- filename: blazephoenix-xyz-health-api-openapi.yml
  format: yaml
  label: BlazePhoenix Health API
  slug: blazephoenix-xyz-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazephoenix-xyz/openapi/blazephoenix-xyz-health-api-openapi.yml
- filename: blazephoenix-xyz-manifest-api-openapi.yml
  format: yaml
  label: BlazePhoenix Manifest API
  slug: blazephoenix-xyz-manifest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazephoenix-xyz/openapi/blazephoenix-xyz-manifest-api-openapi.yml
- filename: blazephoenix-xyz-quote-api-openapi.yml
  format: yaml
  label: BlazePhoenix Quote API
  slug: blazephoenix-xyz-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazephoenix-xyz/openapi/blazephoenix-xyz-quote-api-openapi.yml
- filename: blazephoenix-xyz-stats-api-openapi.yml
  format: yaml
  label: BlazePhoenix Stats API
  slug: blazephoenix-xyz-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazephoenix-xyz/openapi/blazephoenix-xyz-stats-api-openapi.yml
- filename: blazephoenix-xyz-verify-api-openapi.yml
  format: yaml
  label: BlazePhoenix Verify API
  slug: blazephoenix-xyz-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blazephoenix-xyz/openapi/blazephoenix-xyz-verify-api-openapi.yml
consequence_counts:
  read: 11
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Blazephoenix Xyz Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'BlazePhoenix exposes 13 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BlazePhoenix
provider_slug: blazephoenix-xyz
slug: blazephoenix-xyz-agentic-access
source_filename: blazephoenix-xyz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/blazephoenix-xyz-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 11\n    acting: 2\n  by_consequence:\n    read: 11\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/quote/prepare\n  method: get\n  operationId: prepareQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/quote/prepare\n  method: post\n  operationId: prepareQuoteBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/quote/decode\n  method: post\n  operationId: decodeQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/deployments\n  method: get\n  operationId: getDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/abi\n  method: get\n  operationId: getAbi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/quote\n  method: get\n  operationId: getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/quote/batch\n  method: post\n  operationId: getQuoteBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/manifest\n  method: get\n  operationId: getManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api\n  method: get\n  operationId: getDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/badge\n  method: get\n  operationId: getBadge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/verify\n  method: get\n  operationId: verifyFact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/blazephoenix-xyz/agentic-access/blazephoenix-xyz-agentic-access.yml
summary_line: 13 operations · 2 acting
tags:
- Company
- DeFi
- Decentralized Exchange
- Aggregator
- Onchain
---

---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 20
api_specs:
- filename: dapper-labs-accounts-api-openapi.yml
  format: yaml
  label: Dapper Labs Accounts API
  slug: dapper-labs-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapper-labs/refs/heads/main/openapi/dapper-labs-accounts-api-openapi.yml
- filename: dapper-labs-blocks-api-openapi.yml
  format: yaml
  label: Dapper Labs Blocks API
  slug: dapper-labs-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapper-labs/refs/heads/main/openapi/dapper-labs-blocks-api-openapi.yml
- filename: dapper-labs-collections-api-openapi.yml
  format: yaml
  label: Dapper Labs Collections API
  slug: dapper-labs-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapper-labs/refs/heads/main/openapi/dapper-labs-collections-api-openapi.yml
- filename: dapper-labs-events-api-openapi.yml
  format: yaml
  label: Dapper Labs Events API
  slug: dapper-labs-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapper-labs/refs/heads/main/openapi/dapper-labs-events-api-openapi.yml
- filename: dapper-labs-execution-receipts-api-openapi.yml
  format: yaml
  label: Dapper Labs Execution Receipts API
  slug: dapper-labs-execution-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapper-labs/refs/heads/main/openapi/dapper-labs-execution-receipts-api-openapi.yml
- filename: dapper-labs-execution-results-api-openapi.yml
  format: yaml
  label: Dapper Labs Execution Results API
  slug: dapper-labs-execution-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapper-labs/refs/heads/main/openapi/dapper-labs-execution-results-api-openapi.yml
- filename: dapper-labs-network-api-openapi.yml
  format: yaml
  label: Dapper Labs Network API
  slug: dapper-labs-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapper-labs/refs/heads/main/openapi/dapper-labs-network-api-openapi.yml
- filename: dapper-labs-nodeversioninfo-api-openapi.yml
  format: yaml
  label: Dapper Labs NodeVersionInfo API
  slug: dapper-labs-nodeversioninfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapper-labs/refs/heads/main/openapi/dapper-labs-nodeversioninfo-api-openapi.yml
- filename: dapper-labs-scripts-api-openapi.yml
  format: yaml
  label: Dapper Labs Scripts API
  slug: dapper-labs-scripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapper-labs/refs/heads/main/openapi/dapper-labs-scripts-api-openapi.yml
- filename: dapper-labs-subscribe-events-api-openapi.yml
  format: yaml
  label: Dapper Labs Subscribe events API
  slug: dapper-labs-subscribe-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapper-labs/refs/heads/main/openapi/dapper-labs-subscribe-events-api-openapi.yml
- filename: dapper-labs-transactions-api-openapi.yml
  format: yaml
  label: Dapper Labs Transactions API
  slug: dapper-labs-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapper-labs/refs/heads/main/openapi/dapper-labs-transactions-api-openapi.yml
consequence_counts:
  read: 20
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dapper Labs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Dapper Labs exposes 22 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dapper Labs
provider_slug: dapper-labs
slug: dapper-labs-agentic-access
source_filename: dapper-labs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/dapper-labs-flow-access-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 20\n    acting: 2\n  by_consequence:\n    read: 20\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /blocks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blocks/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blocks/{id}/payload\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction_results\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction_results/{transaction_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /execution_results\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /execution_results/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /execution_receipts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /execution_receipts/results/{id}\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{address}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{address}/keys/{index}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{address}/keys\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{address}/balance\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scripts\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network/parameters\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /node_version_info\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscribe_events\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dapper-labs/refs/heads/main/agentic-access/dapper-labs-agentic-access.yml
summary_line: 22 operations · 2 acting
tags:
- Company
- Crypto
- Blockchain
- Web3
- NFT
- Flow
- Smart Contracts
- Developer Tools
---

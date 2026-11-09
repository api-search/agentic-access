---
acting_count: 10
action_class_counts:
  acting: 10
api_specs:
- filename: celestia-blob-api-openapi.yml
  format: yaml
  label: Celestia Node Blob API
  slug: celestia-blob-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/celestia/openapi/celestia-blob-api-openapi.yml
- filename: celestia-contact-api-openapi.yml
  format: yaml
  label: Celestia Contact API
  slug: celestia-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/celestia/openapi/celestia-contact-api-openapi.yml
- filename: celestia-health-api-openapi.yml
  format: yaml
  label: Celestia Health API
  slug: celestia-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/celestia/openapi/celestia-health-api-openapi.yml
- filename: celestia-subscribe-api-openapi.yml
  format: yaml
  label: Celestia Subscribe API
  slug: celestia-subscribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/celestia/openapi/celestia-subscribe-api-openapi.yml
consequence_counts:
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Celestia Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Celestia exposes 10 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Celestia
provider_slug: celestia
slug: celestia-agentic-access
source_filename: celestia-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/celestia-blob-api-openapi.yml, openapi/celestia-blobstream-api-openapi.yml,\n  openapi/celestia-da-api-openapi.yml, openapi/celestia-das-api-openapi.yml, openapi/celestia-fraud-api-openapi.yml,\n  openapi/celestia-header-api-openapi.yml, openapi/celestia-node-api-openapi.yml, openapi/celestia-p2-p-api-openapi.yml,\n  openapi/celestia-share-api-openapi.yml, openapi/celestia-state-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 10\n  by_consequence:\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: post\n  operationId: postRoot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: post\n  operationId: postRoot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: post\n  operationId: postRoot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: post\n  operationId: postRoot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: post\n  operationId: postRoot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: post\n  operationId: postRoot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: post\n  operationId: postRoot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: post\n  operationId: postRoot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: post\n  operationId: postRoot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: post\n  operationId: postRoot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/celestia/agentic-access/celestia-agentic-access.yml
summary_line: 10 operations · 10 acting
tags:
- Blockchain
- Data Availability
- Web3
- Infrastructure
- Open Source
- JSON-RPC
- Modular Blockchain
- Rollup
- Cryptography
- Developer Tools
---

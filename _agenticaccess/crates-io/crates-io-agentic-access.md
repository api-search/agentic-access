---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 10
api_specs:
- filename: crates-io-web-api-openapi.yml
  format: yaml
  label: crates.io Web API
  slug: crates-io-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crates-io/refs/heads/main/openapi/crates-io-web-api-openapi.yml
- filename: crates-io-sparse-index-openapi.yml
  format: yaml
  label: crates.io Sparse Index
  slug: crates-io-sparse-index
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crates-io/refs/heads/main/openapi/crates-io-sparse-index-openapi.yml
consequence_counts:
  read: 10
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Crates Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'crates.io exposes 15 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: crates.io
provider_slug: crates-io
slug: crates-io-agentic-access
source_filename: crates-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/crates-io-sparse-index-openapi.yml, openapi/crates-io-web-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 10\n    acting: 5\n  by_consequence:\n    read: 10\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /config.json\n  method: get\n  operationId: getRegistryConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/{crate}\n  method: get\n  operationId: getIndexOneChar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /2/{crate}\n  method: get\n  operationId: getIndexTwoChar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/{first}/{crate}\n  method: get\n  operationId: getIndexThreeChar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{first_two}/{second_two}/{crate}\n  method: get\n  operationId: getIndexLong\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crates\n  method: get\n  operationId: searchCrates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crates/new\n  method: put\n  operationId: publishCrate\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/crates/{crate}\n  method: get\n  operationId: getCrate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crates/{crate}/{version}\n  method: get\n  operationId: getCrateVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crates/{crate}/{version}/download\n  method: get\n  operationId: downloadCrate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crates/{crate}/{version}/yank\n  method: delete\n\
  \  operationId: yankVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/crates/{crate}/{version}/unyank\n  method: put\n  operationId: unyankVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/crates/{crate}/owners\n  method: get\n  operationId: listOwners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crates/{crate}/owners\n  method: put\n  operationId: addOwner\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/crates/{crate}/owners\n  method: delete\n  operationId: removeOwner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crates-io/refs/heads/main/agentic-access/crates-io-agentic-access.yml
summary_line: 15 operations · 5 acting
tags:
- Rust
- Package Registry
- Crates
- Cargo
- Open Source
- Developer Tools
- Rust Foundation
---

---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 17
api_specs:
- filename: kadena-block-api-openapi.yml
  format: yaml
  label: Kadena block API
  slug: kadena-block-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-block-api-openapi.yml
- filename: kadena-blockhash-api-openapi.yml
  format: yaml
  label: Kadena blockhash API
  slug: kadena-blockhash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-blockhash-api-openapi.yml
- filename: kadena-config-api-openapi.yml
  format: yaml
  label: Kadena config API
  slug: kadena-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-config-api-openapi.yml
- filename: kadena-cut-api-openapi.yml
  format: yaml
  label: Kadena cut API
  slug: kadena-cut-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-cut-api-openapi.yml
- filename: kadena-endpoint-listen-api-openapi.yml
  format: yaml
  label: Kadena endpoint-listen API
  slug: kadena-endpoint-listen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-endpoint-listen-api-openapi.yml
- filename: kadena-endpoint-local-api-openapi.yml
  format: yaml
  label: Kadena endpoint-local API
  slug: kadena-endpoint-local-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-endpoint-local-api-openapi.yml
- filename: kadena-endpoint-poll-api-openapi.yml
  format: yaml
  label: Kadena endpoint-poll API
  slug: kadena-endpoint-poll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-endpoint-poll-api-openapi.yml
- filename: kadena-endpoint-private-api-openapi.yml
  format: yaml
  label: Kadena endpoint-private API
  slug: kadena-endpoint-private-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-endpoint-private-api-openapi.yml
- filename: kadena-endpoint-send-api-openapi.yml
  format: yaml
  label: Kadena endpoint-send API
  slug: kadena-endpoint-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-endpoint-send-api-openapi.yml
- filename: kadena-endpoint-spv-api-openapi.yml
  format: yaml
  label: Kadena endpoint-spv API
  slug: kadena-endpoint-spv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-endpoint-spv-api-openapi.yml
- filename: kadena-header-api-openapi.yml
  format: yaml
  label: Kadena header API
  slug: kadena-header-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-header-api-openapi.yml
- filename: kadena-mempool-api-openapi.yml
  format: yaml
  label: Kadena mempool API
  slug: kadena-mempool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-mempool-api-openapi.yml
- filename: kadena-mining-api-openapi.yml
  format: yaml
  label: Kadena mining API
  slug: kadena-mining-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-mining-api-openapi.yml
- filename: kadena-misc-api-openapi.yml
  format: yaml
  label: Kadena misc API
  slug: kadena-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-misc-api-openapi.yml
- filename: kadena-payload-api-openapi.yml
  format: yaml
  label: Kadena payload API
  slug: kadena-payload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-payload-api-openapi.yml
- filename: kadena-peer-api-openapi.yml
  format: yaml
  label: Kadena peer API
  slug: kadena-peer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-peer-api-openapi.yml
consequence_counts:
  physical: 1
  read: 17
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kadena Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send
operation_count: 37
overview: 'Kadena exposes 37 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 19 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kadena
provider_slug: kadena
slug: kadena-agentic-access
source_filename: kadena-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/kadena-chainweb-openapi-original.yml, openapi/kadena-pact-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 17\n    acting: 20\n  by_consequence:\n    read: 17\n    write: 19\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /cut\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cut\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cut/peer\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cut/peer\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain/{chain}/hash\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/hash/branch\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain/{chain}/block\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/block/branch\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain/{chain}/header\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/header/{blockHash}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /chain/{chain}/header/branch\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain/{chain}/payload/{payloadHash}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/payload/batch\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain/{chain}/payload/{payloadHash}/outputs\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/payload/outputs/batch\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain/{chain}/mempool/getPending\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain/{chain}/mempool/member\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain/{chain}/mempool/lookup\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain/{chain}/mempool/insert\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain/{chain}/mempool/peer\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/mempool/peer\n  method: put\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mining/work\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chainweb/0.0/mainnet01/mining/solved\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mining/updates\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config\n  method: get\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /make-backup\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-backup/{backupId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health-check\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /header/updates\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /block/updates\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /local\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /send\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /poll\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listen\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /private\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spv\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/agentic-access/kadena-agentic-access.yml
summary_line: 37 operations · 20 acting
tags:
- Company
- Crypto Web3
- Blockchain
- Smart Contracts
- Proof of Work
- Layer 1
- Web3
- Cryptocurrency
- Developer Tools
- Decentralized
---

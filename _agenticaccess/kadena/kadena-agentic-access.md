---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 25
api_specs:
- filename: kadena-block-api-openapi.yml
  format: yaml
  label: Kadena Block API
  slug: kadena-block-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-block-api-openapi.yml
- filename: kadena-blockhash-api-openapi.yml
  format: yaml
  label: Kadena Blockhash API
  slug: kadena-blockhash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-blockhash-api-openapi.yml
- filename: kadena-config-api-openapi.yml
  format: yaml
  label: Kadena Config API
  slug: kadena-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-config-api-openapi.yml
- filename: kadena-cut-api-openapi.yml
  format: yaml
  label: Kadena Cut API
  slug: kadena-cut-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-cut-api-openapi.yml
- filename: kadena-endpoint-listen-api-openapi.yml
  format: yaml
  label: Kadena Endpoint Listen API
  slug: kadena-endpoint-listen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-endpoint-listen-api-openapi.yml
- filename: kadena-endpoint-local-api-openapi.yml
  format: yaml
  label: Kadena Endpoint Local API
  slug: kadena-endpoint-local-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-endpoint-local-api-openapi.yml
- filename: kadena-endpoint-poll-api-openapi.yml
  format: yaml
  label: Kadena Endpoint Poll API
  slug: kadena-endpoint-poll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-endpoint-poll-api-openapi.yml
- filename: kadena-endpoint-private-api-openapi.yml
  format: yaml
  label: Kadena Endpoint Private API
  slug: kadena-endpoint-private-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-endpoint-private-api-openapi.yml
- filename: kadena-endpoint-send-api-openapi.yml
  format: yaml
  label: Kadena Endpoint Send API
  slug: kadena-endpoint-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-endpoint-send-api-openapi.yml
- filename: kadena-endpoint-spv-api-openapi.yml
  format: yaml
  label: Kadena Endpoint Spv API
  slug: kadena-endpoint-spv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-endpoint-spv-api-openapi.yml
- filename: kadena-header-api-openapi.yml
  format: yaml
  label: Kadena Header API
  slug: kadena-header-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-header-api-openapi.yml
- filename: kadena-mempool-api-openapi.yml
  format: yaml
  label: Kadena Mempool API
  slug: kadena-mempool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-mempool-api-openapi.yml
- filename: kadena-mining-api-openapi.yml
  format: yaml
  label: Kadena Mining API
  slug: kadena-mining-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-mining-api-openapi.yml
- filename: kadena-misc-api-openapi.yml
  format: yaml
  label: Kadena Misc API
  slug: kadena-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-misc-api-openapi.yml
- filename: kadena-payload-api-openapi.yml
  format: yaml
  label: Kadena Payload API
  slug: kadena-payload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-payload-api-openapi.yml
- filename: kadena-peer-api-openapi.yml
  format: yaml
  label: Kadena Peer API
  slug: kadena-peer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-peer-api-openapi.yml
consequence_counts:
  physical: 1
  read: 25
  write: 12
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
operation_count: 38
overview: 'Kadena exposes 38 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 12 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kadena
provider_slug: kadena
slug: kadena-agentic-access
source_filename: kadena-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/kadena-block-api-openapi.yml, openapi/kadena-blockhash-api-openapi.yml, openapi/kadena-config-api-openapi.yml,\n  openapi/kadena-cut-api-openapi.yml, openapi/kadena-endpoint-listen-api-openapi.yml, openapi/kadena-endpoint-local-api-openapi.yml,\n  openapi/kadena-endpoint-poll-api-openapi.yml, openapi/kadena-endpoint-private-api-openapi.yml,\n  openapi/kadena-endpoint-send-api-openapi.yml, openapi/kadena-endpoint-spv-api-openapi.yml,\n  openapi/kadena-header-api-openapi.yml, openapi/kadena-mempool-api-openapi.yml, openapi/kadena-mining-api-openapi.yml,\n  openapi/kadena-misc-api-openapi.yml, openapi/kadena-payload-api-openapi.yml, openapi/kadena-peer-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\n\
  summary:\n  operations: 38\n  by_action_class:\n    connected: 25\n    acting: 13\n  by_consequence:\n    read: 25\n    write: 12\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /chain/{chain}/block\n  method: get\n  operationId: getChainByChainBlock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/block/branch\n  method: post\n  operationId: postChainByChainBlockBranch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/hash\n  method: get\n  operationId: getChainByChainHash\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/hash/branch\n  method: post\n  operationId: postChainByChainHashBranch\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config\n  method: get\n  operationId: getConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cut\n  method: get\n  operationId: getCut\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cut\n  method: put\n  operationId: putCut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listen\n  method: post\n  operationId: postListen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /local\n  method: post\n  operationId: postLocal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /poll\n  method: post\n  operationId: postPoll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /private\n  method: post\n  operationId: postPrivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /send\n  method: post\n  operationId: postSend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spv\n  method: post\n  operationId: postSpv\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain/{chain}/header\n  method: get\n  operationId: getChainByChainHeader\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/header/{blockHash}\n  method: get\n  operationId: getChainByChainHeaderByBlockHash\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/header/branch\n  method: post\n  operationId: postChainByChainHeaderBranch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/mempool/getPending\n  method: post\n  operationId: postChainByChainMempoolGetPending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/mempool/member\n  method: post\n  operationId: postChainByChainMempoolMember\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain/{chain}/mempool/lookup\n  method: post\n  operationId: postChainByChainMempoolLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/mempool/insert\n  method: put\n  operationId: putChainByChainMempoolInsert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mining/work\n  method: get\n  operationId: getMiningWork\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chainweb/0.0/mainnet01/mining/solved\n  method: post\n  operationId: postChainweb00Mainnet01MiningSolved\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mining/updates\n  method: get\n  operationId: getMiningUpdates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config\n  method: get\n  operationId: getConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /make-backup\n  method: post\n  operationId: postMakeBackup\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-backup/{backupId}\n  method: get\n  operationId: getCheckBackupByBackupId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health-check\n  method: get\n  operationId: getHealthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info\n  method: get\n  operationId: getInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /header/updates\n  method: get\n  operationId: getHeaderUpdates\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /block/updates\n  method: get\n  operationId: getBlockUpdates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/payload/{payloadHash}\n  method: get\n  operationId: getChainByChainPayloadByPayloadHash\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/payload/batch\n  method: post\n  operationId: postChainByChainPayloadBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/payload/{payloadHash}/outputs\n  method: get\n  operationId: getChainByChainPayloadByPayloadHashOutputs\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/payload/outputs/batch\n  method: post\n  operationId: postChainByChainPayloadOutputsBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cut/peer\n  method: get\n  operationId: getCutPeer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cut/peer\n  method: put\n  operationId: putCutPeer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain/{chain}/mempool/peer\n  method: get\n  operationId: getChainByChainMempoolPeer\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/{chain}/mempool/peer\n  method: put\n  operationId: putChainByChainMempoolPeer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/agentic-access/kadena-agentic-access.yml
summary_line: 38 operations · 13 acting
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

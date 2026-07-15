---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 7
api_specs:
- filename: ditto-live-cloud-http-api-openapi.yml
  format: yaml
  label: Ditto Cloud HTTP API
  slug: cloud-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/openapi/ditto-live-cloud-http-api-openapi.yml
- filename: ditto-live-operator-api-openapi.yml
  format: yaml
  label: Ditto Edge Server HTTP API
  slug: edge-server-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/openapi/ditto-live-operator-api-openapi.yml
consequence_counts:
  read: 7
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ditto Live Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Ditto exposes 27 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 20 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ditto
provider_slug: ditto-live
slug: ditto-live-agentic-access
source_filename: ditto-live-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ditto-live-cloud-http-api-openapi.yml, openapi/ditto-live-operator-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    acting: 20\n    connected: 7\n  by_consequence:\n    write: 20\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /store/count\n  method: post\n  operationId: count_endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /store/execute\n  method: post\n  operationId: execute_endpoint\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /store/find\n  method: post\n  operationId: find_endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /store/findbyid\n  method: post\n  operationId: find_by_id_endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /store/write\n \
  \ method: post\n  operationId: write_endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sync/remote_execute\n  method: post\n  operationId: remote_execute_endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app\n  method: get\n  operationId: listApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app\n  method:\
  \ post\n  operationId: createApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}\n  method: get\n  operationId: getApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}\n  method: put\n  operationId: updateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}\n\
  \  method: delete\n  operationId: deleteApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}\n  method: patch\n  operationId: updateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}/apiKey\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}/apiKey\n\
  \  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}/apiKey/{api_key_name}\n  method: get\n  operationId: getApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}/apiKey/{api_key_name}\n  method: delete\n  operationId: deleteApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}/bigPeerReplication\n  method: post\n  operationId: createReplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}/bigPeerReplication/{replication_name}\n  method: get\n  operationId: getReplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}/bigPeerReplication/{replication_name}\n  method: put\n  operationId: updateReplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}/bigPeerReplication/{replication_name}\n  method: delete\n  operationId: deleteReplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}/bigPeerReplication/{replication_name}\n  method: patch\n  operationId: updateReplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}/dataBridge\n  method: get\n  operationId: listDataBridges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}/dataBridge\n  method: post\n  operationId: createDataBridge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}/dataBridge/{data_bridge_name}\n  method: get\n  operationId: getDataBridge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}/dataBridge/{data_bridge_name}\n  method: delete\n  operationId: deleteDataBridge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}/provider\n  method: post\n  operationId: createProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespace/{namespace}/bigPeer/{big_peer_name}/app/{app_name}/provider/{provider_name}\n  method: post\n  operationId: deleteProviderPost\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/agentic-access/ditto-live-agentic-access.yml
summary_line: 27 operations · 20 acting
tags:
- Developer Tools
- Database
- Synchronization
- Peer-to-Peer
- Edge Computing
- Offline-First
- Mobile
---

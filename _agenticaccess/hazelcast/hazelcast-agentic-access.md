---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 11
api_specs:
- filename: hazelcast-openapi.yml
  format: yaml
  label: Hazelcast REST API
  slug: hazelcast-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hazelcast/refs/heads/main/openapi/hazelcast-openapi.yml
consequence_counts:
  read: 11
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hazelcast Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Hazelcast exposes 19 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hazelcast
provider_slug: hazelcast
slug: hazelcast-agentic-access
source_filename: hazelcast-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hazelcast-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 11\n    acting: 8\n  by_consequence:\n    read: 11\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /hazelcast/rest/maps/{mapName}/{key}\n  method: get\n  operationId: getMapEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hazelcast/rest/maps/{mapName}/{key}\n  method: post\n  operationId: putMapEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hazelcast/rest/maps/{mapName}/{key}\n  method: delete\n  operationId: deleteMapEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hazelcast/rest/maps/{mapName}\n  method: delete\n  operationId: clearMap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hazelcast/rest/queues/{queueName}\n  method: post\n  operationId: offerQueueItem\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hazelcast/rest/queues/{queueName}\n  method: delete\n  operationId: pollQueueItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hazelcast/rest/queues/{queueName}/size\n  method: get\n  operationId: getQueueSize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hazelcast/rest/cluster\n  method: get\n  operationId: getClusterInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hazelcast/rest/instance\n  method: get\n  operationId: getInstanceName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hazelcast/rest/management/cluster/state\n  method: get\n  operationId: getClusterState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hazelcast/rest/management/cluster/state\n  method: post\n  operationId: changeClusterState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hazelcast/rest/management/cluster/version\n  method: get\n  operationId: getClusterVersion\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hazelcast/health/ready\n  method: get\n  operationId: healthReady\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hazelcast/health/node-state\n  method: get\n  operationId: healthNodeState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hazelcast/health/cluster-state\n  method: get\n  operationId: healthClusterState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hazelcast/health/cluster-safe\n  method: get\n  operationId: healthClusterSafe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hazelcast/rest/config/reload\n  method: post\n  operationId: reloadConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hazelcast/rest/config/tcp-ip/member-list\n  method: get\n  operationId: getTcpIpMemberList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hazelcast/rest/config/tcp-ip/member-list\n  method: post\n  operationId: updateTcpIpMemberList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hazelcast/refs/heads/main/agentic-access/hazelcast-agentic-access.yml
summary_line: 19 operations · 8 acting
tags:
- Data Caching
- Distributed Computing
- In-Memory Computing
- Real-Time
- REST
---

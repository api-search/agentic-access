---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: nats-monitoring-api-openapi.yml
  format: yaml
  label: NATS Monitoring API
  slug: nats-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nats/refs/heads/main/properties/nats-monitoring-api-openapi.yml
- filename: nats-messaging-asyncapi.yml
  format: yaml
  label: NATS Messaging API
  slug: nats-messaging-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nats/refs/heads/main/properties/nats-messaging-asyncapi.yml
- filename: nats-jetstream-api-asyncapi.yml
  format: yaml
  label: NATS JetStream Management API
  slug: nats-jetstream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nats/refs/heads/main/properties/nats-jetstream-api-asyncapi.yml
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nats Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'NATS exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NATS
provider_slug: nats
slug: nats-agentic-access
source_filename: nats-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nats-monitoring.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /varz\n  method: get\n  operationId: getVarz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connz\n  method: get\n  operationId: getConnz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routez\n  method: get\n  operationId: getRoutez\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gatewayz\n  method: get\n  operationId: getGatewayz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leafz\n  method: get\n  operationId: getLeafz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subsz\n  method: get\n  operationId: getSubsz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jsz\n  method: get\n  operationId: getJsz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accountz\n  method: get\n  operationId: getAccountz\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /healthz\n  method: get\n  operationId: getHealthz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ipqueuesz\n  method: get\n  operationId: getIpqueuesz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nats/refs/heads/main/agentic-access/nats-agentic-access.yml
summary_line: 10 operations
tags:
- Cloud Native
- IoT
- Message Broker
- Microservices
- Pub Sub
---

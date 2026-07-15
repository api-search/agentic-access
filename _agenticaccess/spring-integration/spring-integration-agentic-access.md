---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 9
api_specs:
- filename: spring-integration-http-openapi.yml
  format: yaml
  label: Spring Integration HTTP Adapter API
  slug: spring-integration-http
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-integration/refs/heads/main/openapi/spring-integration-http-openapi.yml
- filename: spring-integration-management-openapi.yml
  format: yaml
  label: Spring Integration Management API
  slug: spring-integration-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-integration/refs/heads/main/openapi/spring-integration-management-openapi.yml
consequence_counts:
  physical: 3
  read: 9
  safety-critical: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Spring Integration Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /controlBus
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /inboundChannelAdapters/{name}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /integration/gateway
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /integration/gateway/{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /integration/inbound
operation_count: 14
overview: 'Spring Integration exposes 14 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 3 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Spring Integration
provider_slug: spring-integration
slug: spring-integration-agentic-access
source_filename: spring-integration-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/spring-integration-http-openapi.yml, openapi/spring-integration-management-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 5\n    connected: 9\n  by_consequence:\n    physical: 3\n    read: 9\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /integration/inbound\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /integration/gateway\n  method: post\n  operationId: sendAndReceive\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/gateway/{path}\n  method: get\n  operationId: sendGetRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integration/gateway/{path}\n  method: post\n  operationId: sendPostRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channels\n  method: get\n  operationId: listChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels/{name}\n  method: get\n  operationId: getChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /handlers\n  method: get\n  operationId: listHandlers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /handlers/{name}\n  method: get\n  operationId: getHandler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inboundChannelAdapters\n  method: get\n  operationId: listInboundAdapters\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inboundChannelAdapters/{name}\n  method: get\n  operationId: getInboundAdapter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inboundChannelAdapters/{name}\n  method: post\n  operationId: controlInboundAdapter\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /graph\n  method: get\n  operationId: getIntegrationGraph\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /messageHistory\n  method: get\n  operationId: getMessageHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /controlBus\n  method: post\n  operationId: sendControlBusCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spring-integration/refs/heads/main/agentic-access/spring-integration-agentic-access.yml
summary_line: 14 operations · 5 acting · 2 human-in-the-loop
tags:
- AMQP
- Enterprise Integration
- Event-Driven
- Integration Patterns
- Java
- Messaging
- Spring
---

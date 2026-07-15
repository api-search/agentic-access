---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 5
api_specs:
- filename: quix-openapi.yml
  format: yaml
  label: Quix Streaming Writer API
  slug: streaming-writer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quix/refs/heads/main/openapi/quix-openapi.yml
- filename: quix-asyncapi.yml
  format: yaml
  label: Quix Streaming Reader API (Real-time)
  slug: streaming-reader-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/quix/refs/heads/main/asyncapi/quix-asyncapi.yml
- filename: quix-openapi.yml
  format: yaml
  label: Quix Portal API (Management)
  slug: portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quix/refs/heads/main/openapi/quix-openapi.yml
- filename: quix-openapi.yml
  format: yaml
  label: Quix Topics & Deployments API
  slug: topics-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quix/refs/heads/main/openapi/quix-openapi.yml
consequence_counts:
  physical: 4
  read: 5
  safety-critical: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Quix Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /deployments/{deploymentId}/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /deployments/{deploymentId}/start
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /topics/{topicName}/streams/{streamId}/events/data
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /topics/{topicName}/streams/{streamId}/parameters/data
operation_count: 16
overview: 'Quix exposes 16 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 6 write, 4 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Quix
provider_slug: quix
slug: quix-agentic-access
source_filename: quix-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/quix-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 11\n    connected: 5\n  by_consequence:\n    write: 6\n    physical: 4\n    read: 5\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /topics/{topicName}/streams\n  method: post\n  operationId: createStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /topics/{topicName}/streams/{streamId}/parameters/data\n  method: post\n\
  \  operationId: sendParameterData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /topics/{topicName}/streams/{streamId}/events/data\n  method: post\n  operationId: sendEventData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /topics/{topicName}/streams/{streamId}/parameters/definitions\n  method: post\n  operationId: setParameterDefinitions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /topics/{topicName}/streams/{streamId}/events/definitions\n  method: post\n  operationId: setEventDefinitions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /topics/{topicName}/streams/{streamId}/close\n  method: post\n  operationId: closeStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces\n\
  \  method: get\n  operationId: getWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}\n  method: get\n  operationId: getWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /topics\n  method: get\n  operationId: getTopics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /topics\n  method: post\n  operationId: createTopic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /topics/{topicId}\n  method: delete\n\
  \  operationId: deleteTopic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments\n  method: get\n  operationId: getDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployments\n  method: post\n  operationId: createDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/{deploymentId}\n  method: get\n  operationId: getDeployment\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployments/{deploymentId}/start\n  method: put\n  operationId: startDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/{deploymentId}/stop\n  method: put\n  operationId: stopDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quix/refs/heads/main/agentic-access/quix-agentic-access.yml
summary_line: 16 operations · 11 acting · 1 human-in-the-loop
tags:
- Stream Processing
- Real Time
- Kafka
- Python
- Streaming Data
---

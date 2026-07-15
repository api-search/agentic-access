---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 1
api_specs:
- filename: beam-cloud-openapi.yml
  format: yaml
  label: Beam Web Endpoints API
  slug: beam-cloud-web-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-cloud/refs/heads/main/openapi/beam-cloud-openapi.yml
- filename: beam-cloud-openapi.yml
  format: yaml
  label: Beam Task Queues API
  slug: beam-cloud-task-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-cloud/refs/heads/main/openapi/beam-cloud-openapi.yml
- filename: beam-cloud-openapi.yml
  format: yaml
  label: Beam Tasks Management API
  slug: beam-cloud-tasks-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-cloud/refs/heads/main/openapi/beam-cloud-openapi.yml
- filename: beam-cloud-openapi.yml
  format: yaml
  label: Beam Sandboxes and Volumes API
  slug: beam-cloud-sandboxes-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-cloud/refs/heads/main/openapi/beam-cloud-openapi.yml
consequence_counts:
  physical: 4
  read: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Beam Cloud Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /endpoint/id/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /endpoint/{name}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /endpoint/{name}/v{version}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /taskqueue/{name}
operation_count: 6
overview: 'Beam exposes 6 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 1 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Beam
provider_slug: beam-cloud
slug: beam-cloud-agentic-access
source_filename: beam-cloud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/beam-cloud-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 5\n    connected: 1\n  by_consequence:\n    physical: 4\n    read: 1\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /endpoint/{name}\n  method: post\n  operationId: invokeNamedEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /endpoint/{name}/v{version}\n  method:\
  \ post\n  operationId: invokeNamedEndpointVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /endpoint/id/{id}\n  method: post\n  operationId: invokeEndpointById\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /taskqueue/{name}\n  method: post\n  operationId: submitTaskByName\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/task/{task_id}/\n  method: get\n  operationId: getTaskStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/task/cancel/\n  method: delete\n  operationId: cancelTasks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beam-cloud/refs/heads/main/agentic-access/beam-cloud-agentic-access.yml
summary_line: 6 operations · 5 acting
tags:
- Serverless
- GPU
- Python
- Inference
- Containers
---

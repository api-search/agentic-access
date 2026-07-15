---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 4
api_specs:
- filename: tensordock-marketplace-api-openapi.yml
  format: yaml
  label: TensorDock Marketplace API
  slug: tensordock-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-marketplace-api-openapi.yml
- filename: tensordock-instances-api-openapi.yml
  format: yaml
  label: TensorDock Instances API
  slug: tensordock-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-instances-api-openapi.yml
- filename: tensordock-secrets-api-openapi.yml
  format: yaml
  label: TensorDock Secrets API
  slug: tensordock-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-secrets-api-openapi.yml
consequence_counts:
  read: 4
  safety-critical: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Tensordock Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/instances/{id}/stop
operation_count: 11
overview: 'TensorDock exposes 11 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 6 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TensorDock
provider_slug: tensordock
slug: tensordock-agentic-access
source_filename: tensordock-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tensordock-instances-api-openapi.yml, openapi/tensordock-secrets-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 4\n    acting: 7\n  by_consequence:\n    read: 4\n    write: 6\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v2/instances\n  method: get\n  operationId: listInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/instances\n  method: post\n  operationId: createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/instances/{id}\n  method: get\n  operationId: getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/instances/{id}\n  method: delete\n  operationId: deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/instances/{id}/start\n  method: post\n  operationId: startInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/instances/{id}/stop\n  method: post\n  operationId: stopInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/instances/{id}/modify\n  method: put\n  operationId: modifyInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/secrets\n  method: get\n  operationId: listSecrets\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/secrets\n  method: post\n  operationId: createSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/secrets/{id}\n  method: get\n  operationId: getSecret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/secrets/{id}\n  method: delete\n  operationId: deleteSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/agentic-access/tensordock-agentic-access.yml
summary_line: 11 operations · 7 acting · 1 human-in-the-loop
tags:
- GPU
- Cloud
- Marketplace
- Compute
- Virtual Machines
- AI
- Machine Learning
- Bare Metal
- Spot Instances
- Containers
---

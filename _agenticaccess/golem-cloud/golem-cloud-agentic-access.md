---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 14
api_specs:
- filename: golem-cloud-openapi.yml
  format: yaml
  label: Golem Components API
  slug: components
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golem-cloud/refs/heads/main/openapi/golem-cloud-openapi.yml
- filename: golem-cloud-openapi.yml
  format: yaml
  label: Golem Workers & Invocation API
  slug: workers-invocation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golem-cloud/refs/heads/main/openapi/golem-cloud-openapi.yml
- filename: golem-cloud-openapi.yml
  format: yaml
  label: Golem API Definitions & Deployments API
  slug: api-definitions-deployments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golem-cloud/refs/heads/main/openapi/golem-cloud-openapi.yml
- filename: golem-cloud-openapi.yml
  format: yaml
  label: Golem Plugins API
  slug: plugins
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golem-cloud/refs/heads/main/openapi/golem-cloud-openapi.yml
consequence_counts:
  physical: 2
  read: 14
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Golem Cloud Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/api/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/api/deployments/{site}
operation_count: 33
overview: 'Golem exposes 33 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 17 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Golem
provider_slug: golem-cloud
slug: golem-cloud-agentic-access
source_filename: golem-cloud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/golem-cloud-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    acting: 19\n    connected: 14\n  by_consequence:\n    write: 17\n    read: 14\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/envs/{environment_id}/components\n  method: post\n  operationId: createComponent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/envs/{environment_id}/components\n  method: get\n  operationId: listEnvironmentComponents\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/envs/{environment_id}/components/{component_name}\n  method: get\n  operationId: getComponentByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/components/{component_id}\n  method: get\n  operationId: getComponent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/components/{component_id}\n  method: patch\n  operationId: updateComponent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/components/{component_id}\n  method: delete\n  operationId: deleteComponent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/components/{component_id}/revisions/{revision}/wasm\n  method: get\n  operationId: downloadComponentWasm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/components/{component_id}/workers\n  method: post\n  operationId: launchNewWorker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/components/{component_id}/workers\n  method: get\n  operationId: getWorkersMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/components/{component_id}/workers/{agent_name}\n  method: get\n  operationId: getWorkerMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/components/{component_id}/workers/{agent_name}\n  method: delete\n  operationId: deleteWorker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/components/{component_id}/workers/{agent_name}/invoke\n  method: post\n  operationId: invokeFunction\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/components/{component_id}/workers/{agent_name}/invoke-and-await\n  method: post\n  operationId: invokeAndAwaitFunction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/components/{component_id}/workers/{agent_name}/interrupt\n  method: post\n  operationId: interruptWorker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/components/{component_id}/workers/{agent_name}/resume\n  method: post\n  operationId: resumeWorker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/components/{component_id}/workers/{agent_name}/update\n  method: post\n  operationId: updateWorker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/components/{component_id}/workers/{agent_name}/oplog\n  method: get\n  operationId: getOplog\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/components/{component_id}/workers/{agent_name}/connect\n  method: get\n  operationId: connectWorker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/definitions\n  method: get\n  operationId: listApiDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/definitions\n  method: post\n  operationId: createApiDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/definitions/{id}/{version}\n  method: get\n  operationId: getApiDefinition\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/definitions/{id}/{version}\n  method: put\n  operationId: updateApiDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/definitions/{id}/{version}\n  method: delete\n  operationId: deleteApiDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/deployments\n  method: get\n  operationId: listApiDeployments\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/deployments\n  method: post\n  operationId: deployApiDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/deployments/{site}\n  method: get\n  operationId: getApiDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/deployments/{site}\n  method: delete\n  operationId: deleteApiDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/plugins\n  method: get\n  operationId: listPlugins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/plugins\n  method: post\n  operationId: createPlugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/plugins/{plugin_id}\n  method: get\n  operationId: getPlugin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/plugins/{plugin_id}\n\
  \  method: delete\n  operationId: deletePlugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/components/{component_id}/workers/{agent_name}/activate-plugin\n  method: post\n  operationId: activatePlugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/components/{component_id}/workers/{agent_name}/deactivate-plugin\n  method: post\n  operationId: deactivatePlugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/golem-cloud/refs/heads/main/agentic-access/golem-cloud-agentic-access.yml
summary_line: 33 operations · 19 acting
tags:
- Durable Computing
- Serverless
- WebAssembly
- Workers
- Agents
---

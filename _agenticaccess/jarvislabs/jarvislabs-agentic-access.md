---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 6
api_specs:
- filename: jarvislabs-openapi.yml
  format: yaml
  label: JarvisLabs Instances API
  slug: jarvislabs-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/openapi/jarvislabs-openapi.yml
- filename: jarvislabs-openapi.yml
  format: yaml
  label: JarvisLabs GPU Types API
  slug: jarvislabs-gpu-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/openapi/jarvislabs-openapi.yml
- filename: jarvislabs-openapi.yml
  format: yaml
  label: JarvisLabs Templates API
  slug: jarvislabs-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/openapi/jarvislabs-openapi.yml
- filename: jarvislabs-openapi.yml
  format: yaml
  label: JarvisLabs Inference & Deploy API
  slug: jarvislabs-inference-deploy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/openapi/jarvislabs-openapi.yml
- filename: jarvislabs-openapi.yml
  format: yaml
  label: JarvisLabs SDK & CLI
  slug: jarvislabs-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/openapi/jarvislabs-openapi.yml
consequence_counts:
  read: 6
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Jarvislabs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'JarvisLabs exposes 13 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: JarvisLabs
provider_slug: jarvislabs
slug: jarvislabs-agentic-access
source_filename: jarvislabs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/jarvislabs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 6\n    acting: 7\n  by_consequence:\n    read: 6\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /instances\n  method: get\n  operationId: listInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances\n  method: post\n  operationId: createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{machine_id}\n  method: get\n  operationId: getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances/{machine_id}\n  method: patch\n  operationId: renameInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{machine_id}\n  method: delete\n  operationId: destroyInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /instances/{machine_id}/pause\n  method: post\n  operationId: pauseInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{machine_id}/resume\n  method: post\n  operationId: resumeInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gpus\n  method: get\n  operationId: listGpuTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates\n  method: get\n  operationId:\
  \ listTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /filesystems\n  method: get\n  operationId: listFilesystems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /filesystems\n  method: post\n  operationId: createFilesystem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /filesystems/{fs_id}\n  method: delete\n  operationId: deleteFilesystem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/balance\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/agentic-access/jarvislabs-agentic-access.yml
summary_line: 13 operations · 7 acting
tags:
- AI
- GPU
- Cloud
- Infrastructure
- Compute
---

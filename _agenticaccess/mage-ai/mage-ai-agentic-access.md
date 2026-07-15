---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 6
api_specs:
- filename: mage-ai-openapi.yml
  format: yaml
  label: Mage Pipeline Triggers & Runs API
  slug: pipeline-triggers-runs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mage-ai/refs/heads/main/openapi/mage-ai-openapi.yml
- filename: mage-ai-openapi.yml
  format: yaml
  label: Mage Pipelines API
  slug: pipelines
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mage-ai/refs/heads/main/openapi/mage-ai-openapi.yml
- filename: mage-ai-openapi.yml
  format: yaml
  label: Mage Blocks API
  slug: blocks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mage-ai/refs/heads/main/openapi/mage-ai-openapi.yml
- filename: mage-ai-openapi.yml
  format: yaml
  label: Mage Pipeline Schedules API
  slug: schedules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mage-ai/refs/heads/main/openapi/mage-ai-openapi.yml
consequence_counts:
  read: 6
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mage Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Mage exposes 15 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mage
provider_slug: mage-ai
slug: mage-ai-agentic-access
source_filename: mage-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/mage-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 9\n    connected: 6\n  by_consequence:\n    write: 9\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /pipeline_schedules/{schedule_id}/pipeline_runs/{token}\n  method: post\n  operationId: triggerPipelineRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipeline_runs\n  method: get\n  operationId: listPipelineRuns\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipeline_runs/{id}\n  method: get\n  operationId: readPipelineRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines\n  method: get\n  operationId: listPipelines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines\n  method: post\n  operationId: createPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{uuid}\n  method: get\n  operationId: readPipeline\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines/{uuid}\n  method: put\n  operationId: updatePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{uuid}\n  method: delete\n  operationId: deletePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{uuid}/blocks\n  method: post\n  operationId: createBlock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{uuid}/blocks/{block_uuid}\n  method: get\n  operationId: readBlock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines/{uuid}/blocks/{block_uuid}\n  method: put\n  operationId: updateBlock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{uuid}/blocks/{block_uuid}\n  method: delete\n  operationId: deleteBlock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipeline_schedules\n  method: get\n  operationId: listPipelineSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines/{uuid}/pipeline_schedules\n  method: post\n  operationId: createPipelineSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipeline_schedules/{id}\n  method: put\n  operationId: updatePipelineSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mage-ai/refs/heads/main/agentic-access/mage-ai-agentic-access.yml
summary_line: 15 operations · 9 acting
tags:
- Data Pipelines
- Orchestration
- ETL
- Data Engineering
- Open Source
---

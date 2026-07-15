---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 6
api_specs:
- filename: y42-openapi.yml
  format: yaml
  label: Y42 Spaces API
  slug: y42-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/y42/refs/heads/main/openapi/y42-openapi.yml
- filename: y42-openapi.yml
  format: yaml
  label: Y42 Orchestration API
  slug: y42-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/y42/refs/heads/main/openapi/y42-openapi.yml
- filename: y42-openapi.yml
  format: yaml
  label: Y42 Runs API
  slug: y42-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/y42/refs/heads/main/openapi/y42-openapi.yml
- filename: y42-openapi.yml
  format: yaml
  label: Y42 Manifest API
  slug: y42-manifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/y42/refs/heads/main/openapi/y42-openapi.yml
consequence_counts:
  read: 6
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Y42 Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Y42 exposes 11 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Y42
provider_slug: y42
slug: y42-agentic-access
source_filename: y42-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/y42-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 6\n    acting: 5\n  by_consequence:\n    read: 6\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/1/github-backend/{org_slug}/\n  method: get\n  operationId: listSpaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1/github-backend/{org_slug}/space\n  method: post\n  operationId: createSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/github-backend/{org_slug}/space/{slug}\n  method: get\n  operationId: getSpace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1/github-backend/{org_slug}/space/{slug}\n  method: delete\n  operationId: deleteSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/github-backend/{org_slug}/space/{slug}/credentials\n  method: patch\n  operationId: updateSpaceCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/credential/{org_slug}/{space_slug}/connections\n  method: post\n  operationId: createConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/4/orchestrations/{org_slug}/{space_slug}\n  method: post\n  operationId: triggerOrchestration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/4/orchestrations/{org_slug}/{space_slug}/run\n  method: get\n  operationId: getOrchestrationRun\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/4/orchestrations/{org_slug}/{space_slug}/runs\n  method: get\n  operationId: listOrchestrationRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1/job-info-service/{org_slug}/{space_slug}/latest-jobs\n  method: get\n  operationId: getLatestJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1/dbt/{org_slug}/{space_slug}/manifest\n  method: get\n  operationId: getManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/y42/refs/heads/main/agentic-access/y42-agentic-access.yml
summary_line: 11 operations · 5 acting
tags:
- DataOps
- Data Pipelines
- Orchestration
- dbt
- Snowflake
- BigQuery
- GitOps
---

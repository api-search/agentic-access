---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 7
api_specs:
- filename: redocly-health-api-openapi.yml
  format: yaml
  label: Redocly Health API
  slug: redocly-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-health-api-openapi.yml
- filename: redocly-metadata-api-openapi.yml
  format: yaml
  label: Redocly Metadata API
  slug: redocly-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-metadata-api-openapi.yml
- filename: redocly-remotes-api-openapi.yml
  format: yaml
  label: Redocly Remotes API
  slug: redocly-remotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-remotes-api-openapi.yml
- filename: redocly-search-api-openapi.yml
  format: yaml
  label: Redocly Search API
  slug: redocly-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-search-api-openapi.yml
- filename: redocly-status-api-openapi.yml
  format: yaml
  label: Redocly Status API
  slug: redocly-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-status-api-openapi.yml
- filename: redocly-tasks-api-openapi.yml
  format: yaml
  label: Redocly Tasks API
  slug: redocly-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-tasks-api-openapi.yml
- filename: redocly-webhooks-api-openapi.yml
  format: yaml
  label: Redocly Webhooks API
  slug: redocly-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-webhooks-api-openapi.yml
- filename: redocly-to-dos-api-openapi.yml
  format: yaml
  label: Redocly To Dos API
  slug: redocly-to-dos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-to-dos-api-openapi.yml
consequence_counts:
  read: 7
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Redocly Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Redocly exposes 15 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Redocly
provider_slug: redocly
slug: redocly-agentic-access
source_filename: redocly-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-04'\nmethod: generated\nsource: openapi/redocly-health-api-openapi.yml, openapi/redocly-metadata-api-openapi.yml, openapi/redocly-remotes-api-openapi.yml,\n  openapi/redocly-search-api-openapi.yml, openapi/redocly-status-api-openapi.yml, openapi/redocly-tasks-api-openapi.yml,\n  openapi/redocly-to-dos-api-openapi.yml, openapi/redocly-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 7\n    acting: 8\n  by_consequence:\n    read: 7\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /orgs/{orgId}/projects/{projectId}/scout/metadata/validate\n  method: post\n  operationId: validateMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/projects/{projectId}/remotes\n  method: post\n  operationId: upsertRemote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/projects/{projectId}/remotes/{remoteId}/push\n  method: post\n  operationId: pushToRemote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /_search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_search-facets\n  method: post\n  operationId: searchFacets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/projects/{projectId}/scout/status\n  method: post\n  operationId: reportStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/projects/{projectId}/scout/tasks\n  method: post\n  operationId: startNextJob\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/projects/{projectId}/scout/tasks\n  method: get\n  operationId: getAllTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/projects/{projectId}/scout/tasks/{jobId}\n  method: get\n  operationId: getJobById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/projects/{projectId}/scout/tasks/{jobId}\n  method: patch\n  operationId: updateJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/projects/{projectId}/scout/todos\n  method: post\n  operationId: createTodo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/projects/{projectId}/scout/todos\n  method: get\n  operationId: getAllTodos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/github\n  method: post\n  operationId: processGithubWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/gitlab\n  method: post\n  operationId: processGitlabWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/agentic-access/redocly-agentic-access.yml
summary_line: 15 operations · 8 acting
tags:
- Artificial Intelligence
- API Catalog
- API Documentation
- Arazzo
- Developer Portal
- Governance
- Linting
- MCP
- Monitoring
- OpenAPI
- A2A
---

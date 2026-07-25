---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 7
api_specs:
- filename: scalable-platforms-artifacts-api-openapi.yml
  format: yaml
  label: Scalable Platforms Artifacts API
  slug: scalable-platforms-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/openapi/scalable-platforms-artifacts-api-openapi.yml
- filename: scalable-platforms-deployments-api-openapi.yml
  format: yaml
  label: Scalable Platforms Deployments API
  slug: scalable-platforms-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/openapi/scalable-platforms-deployments-api-openapi.yml
- filename: scalable-platforms-domains-api-openapi.yml
  format: yaml
  label: Scalable Platforms Domains API
  slug: scalable-platforms-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/openapi/scalable-platforms-domains-api-openapi.yml
- filename: scalable-platforms-environments-api-openapi.yml
  format: yaml
  label: Scalable Platforms Environments API
  slug: scalable-platforms-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/openapi/scalable-platforms-environments-api-openapi.yml
- filename: scalable-platforms-projects-api-openapi.yml
  format: yaml
  label: Scalable Platforms Projects API
  slug: scalable-platforms-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/openapi/scalable-platforms-projects-api-openapi.yml
- filename: scalable-platforms-teams-api-openapi.yml
  format: yaml
  label: Scalable Platforms Teams API
  slug: scalable-platforms-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/openapi/scalable-platforms-teams-api-openapi.yml
consequence_counts:
  physical: 2
  read: 7
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Scalable Platforms Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v13/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v13/deployments/{id}
operation_count: 14
overview: 'Scalable Platforms exposes 14 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 5 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Scalable Platforms
provider_slug: scalable-platforms
slug: scalable-platforms-agentic-access
source_filename: scalable-platforms-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/scalable-platforms-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 7\n    acting: 7\n  by_consequence:\n    read: 7\n    physical: 2\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v6/deployments\n  method: get\n  operationId: listDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v13/deployments\n  method: post\n  operationId: createDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n   \
  \   exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v13/deployments/{id}\n  method: get\n  operationId: getDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v13/deployments/{id}\n  method: delete\n  operationId: deleteDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v9/projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v9/projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/pause\n  method: post\n  operationId: pauseProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/unpause\n  method: post\n  operationId: unpauseProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v9/projects/{idOrName}/customenvironments\n  method: get\n  operationId: listCustomEnvironments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/domains\n  method: get\n  operationId: listDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/domains\n  method: post\n  operationId: addDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v6/domains/{domain}/config\n  method: get\n  operationId: getDomainConfig\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v8/artifacts/{hash}\n  method: put\n  operationId: uploadCacheArtifact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/agentic-access/scalable-platforms-agentic-access.yml
summary_line: 14 operations · 7 acting
tags:
- Cloud Infrastructure
- Deployment
- Developer Experience
- DevOps
- PaaS
- Platform
- Scalability
- Serverless
---

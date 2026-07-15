---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 5
api_specs:
- filename: flightcontrol-openapi.yml
  format: yaml
  label: Flightcontrol Management API
  slug: flightcontrol-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightcontrol/refs/heads/main/openapi/flightcontrol-openapi.yml
- filename: flightcontrol-openapi.yml
  format: yaml
  label: Flightcontrol Deploy Hooks API
  slug: flightcontrol-deploy-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightcontrol/refs/heads/main/openapi/flightcontrol-openapi.yml
- filename: flightcontrol-openapi.yml
  format: yaml
  label: Flightcontrol CloudFront Invalidation API
  slug: flightcontrol-cloudfront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightcontrol/refs/heads/main/openapi/flightcontrol-openapi.yml
consequence_counts:
  read: 5
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Flightcontrol Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Flightcontrol exposes 10 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Flightcontrol
provider_slug: flightcontrol
slug: flightcontrol-agentic-access
source_filename: flightcontrol-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/flightcontrol-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 5\n    acting: 5\n  by_consequence:\n    read: 5\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/deployments/{deploymentId}\n  method: get\n  operationId: getDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/environments\n  method: post\n  operationId: createEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/environments\n  method: patch\n  operationId: editEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/services\n  method: get\n  operationId: getServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/services/{serviceId}/scaling\n  method: post\n  operationId: updateScaling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/environments/{environmentId}/env-variables\n  method: post\n  operationId: createEnvironmentEnvVariables\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/services/{serviceId}/cloudfront/invalidation\n  method: post\n  operationId: createCloudFrontInvalidation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cloudfront/invalidation/{invalidationId}\n  method: get\n  operationId: getCloudFrontInvalidationStatus\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/deploy-hook/{envId}/{secret}\n  method: get\n  operationId: triggerDeployHook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/deploy-hook/{previewEnvId}/{secret}/{prNumber}/{commitSHA}\n  method: get\n  operationId: triggerPreviewDeployHook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flightcontrol/refs/heads/main/agentic-access/flightcontrol-agentic-access.yml
summary_line: 10 operations · 5 acting
tags:
- Deployment
- PaaS
- Infrastructure
- DevOps
---

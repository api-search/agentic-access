---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 12
api_specs:
- filename: buildpulse-io-auth-api-openapi.yml
  format: yaml
  label: BuildPulse Auth API
  slug: buildpulse-io-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-auth-api-openapi.yml
- filename: buildpulse-io-badges-api-openapi.yml
  format: yaml
  label: BuildPulse Badges API
  slug: buildpulse-io-badges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-badges-api-openapi.yml
- filename: buildpulse-io-flaky-api-openapi.yml
  format: yaml
  label: BuildPulse Flaky API
  slug: buildpulse-io-flaky-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-flaky-api-openapi.yml
- filename: buildpulse-io-health-api-openapi.yml
  format: yaml
  label: BuildPulse Health API
  slug: buildpulse-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-health-api-openapi.yml
- filename: buildpulse-io-submissions-api-openapi.yml
  format: yaml
  label: BuildPulse Submissions API
  slug: buildpulse-io-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-submissions-api-openapi.yml
- filename: buildpulse-io-tests-api-openapi.yml
  format: yaml
  label: BuildPulse Tests API
  slug: buildpulse-io-tests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-tests-api-openapi.yml
- filename: buildpulse-io-webhooks-api-openapi.yml
  format: yaml
  label: BuildPulse Webhooks API
  slug: buildpulse-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-webhooks-api-openapi.yml
consequence_counts:
  read: 12
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Buildpulse Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'BuildPulse exposes 13 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BuildPulse
provider_slug: buildpulse-io
slug: buildpulse-io-agentic-access
source_filename: buildpulse-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/buildpulse-io-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 12\n    acting: 1\n  by_consequence:\n    read: 12\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/github\n  method: post\n  operationId: githubWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api\n  method: get\n  operationId: validateToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me/organizations\n  method: get\n  operationId: listMyOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me/repositories\n  method: get\n  operationId: listMyRepositories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{owner}/{name}/submissions\n  method:\
  \ get\n  operationId: listSubmissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{owner}/{name}/submissions/{submission_id}/tests\n  method: get\n  operationId: listSubmissionTests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{owner}/{name}/tests\n  method: get\n  operationId: listTests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tests/{id}/results\n  method: get\n  operationId: listTestResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/flaky/tests\n  method: get\n  operationId: listFlakyTests\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/flaky/badges\n  method: get\n  operationId: flakyBadge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/coverage/badges\n  method: get\n  operationId: coverageBadge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/buildpulse-io/agentic-access/buildpulse-io-agentic-access.yml
summary_line: 13 operations · 1 acting
tags:
- CI
- DevOps
- Testing
- Artificial Intelligence
- Analytics
- Company
---

---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 5
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google Cloud Artifact Registry API
  slug: google-cloud-artifact-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-artifact-registry/refs/heads/main/openapi/openapi.yml
consequence_counts:
  read: 5
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Artifact Registry Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Google Cloud Artifact Registry exposes 8 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Artifact Registry
provider_slug: google-cloud-artifact-registry
slug: google-cloud-artifact-registry-agentic-access
source_filename: google-cloud-artifact-registry-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 5\n    acting: 3\n  by_consequence:\n    read: 5\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/projects/{projectId}/locations\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/locations/{location}/repositories\n  method: get\n  operationId: listRepositories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /v1/projects/{projectId}/locations/{location}/repositories\n  method: post\n  operationId: createRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/locations/{location}/repositories/{repositoryId}\n  method: get\n  operationId: getRepository\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/locations/{location}/repositories/{repositoryId}\n  method: patch\n  operationId: updateRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/locations/{location}/repositories/{repositoryId}\n  method: delete\n  operationId: deleteRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/locations/{location}/repositories/{repositoryId}/packages\n  method: get\n  operationId: listPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/locations/{location}/repositories/{repositoryId}/dockerImages\n  method: get\n  operationId: listDockerImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-artifact-registry/refs/heads/main/agentic-access/google-cloud-artifact-registry-agentic-access.yml
summary_line: 8 operations · 3 acting
tags:
- Artifacts
- Containers
- Docker
- Google Cloud
- Packages
- Registries
- Repositories
- Security
- Supply Chain
---

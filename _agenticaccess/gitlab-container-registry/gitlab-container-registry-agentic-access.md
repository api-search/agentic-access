---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 5
api_specs:
- filename: gitlab-container-registry-repositories-api-openapi.yml
  format: yaml
  label: GitLab Container Registry Repositories API
  slug: gitlab-container-registry-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab-container-registry/refs/heads/main/openapi/gitlab-container-registry-repositories-api-openapi.yml
- filename: gitlab-container-registry-tags-api-openapi.yml
  format: yaml
  label: GitLab Container Registry Tags API
  slug: gitlab-container-registry-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab-container-registry/refs/heads/main/openapi/gitlab-container-registry-tags-api-openapi.yml
consequence_counts:
  read: 5
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gitlab Container Registry Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'GitLab Container Registry exposes 8 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GitLab Container Registry
provider_slug: gitlab-container-registry
slug: gitlab-container-registry-agentic-access
source_filename: gitlab-container-registry-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gitlab-container-registry-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 5\n    acting: 3\n  by_consequence:\n    read: 5\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /registry/repositories/{id}\n  method: get\n  operationId: getRegistryRepository\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api\n- path: /projects/{id}/registry/repositories\n  method: get\n  operationId: listProjectRegistryRepositories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api\n- path: /groups/{id}/registry/repositories\n  method: get\n  operationId: listGroupRegistryRepositories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api\n- path: /projects/{id}/registry/repositories/{repository_id}\n  method: delete\n  operationId: deleteProjectRegistryRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - api\n- path: /projects/{id}/registry/repositories/{repository_id}/tags\n  method: get\n  operationId: listRepositoryTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n    scope:\n    - api\n- path: /projects/{id}/registry/repositories/{repository_id}/tags\n  method: delete\n  operationId: deleteRepositoryTagsBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - api\n- path: /projects/{id}/registry/repositories/{repository_id}/tags/{tag_name}\n  method: get\n  operationId: getRepositoryTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api\n- path: /projects/{id}/registry/repositories/{repository_id}/tags/{tag_name}\n  method: delete\n  operationId: deleteRepositoryTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitlab-container-registry/refs/heads/main/agentic-access/gitlab-container-registry-agentic-access.yml
summary_line: 8 operations · 3 acting
tags:
- Container Images
- Containers
- GitLab
- Registry
---

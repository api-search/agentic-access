---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 12
api_specs:
- filename: google-cloud-platform-folders-api-openapi.yml
  format: yaml
  label: Google Cloud Platform Folders API
  slug: google-cloud-platform-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-folders-api-openapi.yml
- filename: google-cloud-platform-operations-api-openapi.yml
  format: yaml
  label: Google Cloud Platform Operations API
  slug: google-cloud-platform-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-operations-api-openapi.yml
- filename: google-cloud-platform-organizations-api-openapi.yml
  format: yaml
  label: Google Cloud Platform Organizations API
  slug: google-cloud-platform-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-organizations-api-openapi.yml
- filename: google-cloud-platform-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Platform Projects API
  slug: google-cloud-platform-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-projects-api-openapi.yml
- filename: google-cloud-platform-tagbindings-api-openapi.yml
  format: yaml
  label: Google Cloud Platform TagBindings API
  slug: google-cloud-platform-tagbindings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-tagbindings-api-openapi.yml
- filename: google-cloud-platform-tagkeys-api-openapi.yml
  format: yaml
  label: Google Cloud Platform TagKeys API
  slug: google-cloud-platform-tagkeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-tagkeys-api-openapi.yml
- filename: google-cloud-platform-tagvalues-api-openapi.yml
  format: yaml
  label: Google Cloud Platform TagValues API
  slug: google-cloud-platform-tagvalues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-tagvalues-api-openapi.yml
consequence_counts:
  read: 12
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Platform Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'Google Cloud Platform exposes 28 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 16 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
slug: google-cloud-platform-agentic-access
source_filename: google-cloud-platform-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cloud-resource-manager-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 12\n    acting: 16\n  by_consequence:\n    read: 12\n    write: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/projects\n  method: get\n  operationId: cloudresourcemanager.projects.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/projects\n  method: post\n  operationId: cloudresourcemanager.projects.create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/projects/{projectId}\n  method: get\n  operationId: cloudresourcemanager.projects.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/projects/{projectId}\n  method: patch\n  operationId: cloudresourcemanager.projects.patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/projects/{projectId}\n  method: delete\n  operationId: cloudresourcemanager.projects.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/projects/{projectId}:undelete\n  method: post\n  operationId: cloudresourcemanager.projects.undelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/projects/{resource}:getIamPolicy\n  method: post\n  operationId: cloudresourcemanager.projects.getIamPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/projects/{resource}:setIamPolicy\n  method: post\n  operationId: cloudresourcemanager.projects.setIamPolicy\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/projects:search\n  method: get\n  operationId: cloudresourcemanager.projects.search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/folders\n  method: get\n  operationId: cloudresourcemanager.folders.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n\
  \    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/folders\n  method: post\n  operationId: cloudresourcemanager.folders.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/folders/{folderId}\n  method: get\n  operationId: cloudresourcemanager.folders.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/folders/{folderId}\n  method: patch\n  operationId: cloudresourcemanager.folders.patch\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/folders/{folderId}\n  method: delete\n  operationId: cloudresourcemanager.folders.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/folders/{folderId}:undelete\n  method: post\n  operationId: cloudresourcemanager.folders.undelete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/folders/{folderId}:move\n  method: post\n  operationId: cloudresourcemanager.folders.move\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/folders:search\n  method: get\n  operationId: cloudresourcemanager.folders.search\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/organizations/{organizationId}\n  method: get\n  operationId: cloudresourcemanager.organizations.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/organizations:search\n  method: get\n  operationId: cloudresourcemanager.organizations.search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n\
  - path: /v3/organizations/{resource}:getIamPolicy\n  method: post\n  operationId: cloudresourcemanager.organizations.getIamPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/organizations/{resource}:setIamPolicy\n  method: post\n  operationId: cloudresourcemanager.organizations.setIamPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n\
  \    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/{name}\n  method: get\n  operationId: cloudresourcemanager.operations.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/tagKeys\n  method: get\n  operationId: cloudresourcemanager.tagKeys.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/tagKeys\n  method: post\n  operationId: cloudresourcemanager.tagKeys.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/tagValues\n  method: get\n  operationId: cloudresourcemanager.tagValues.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/tagValues\n  method: post\n  operationId: cloudresourcemanager.tagValues.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/tagBindings\n  method: get\n  operationId: cloudresourcemanager.tagBindings.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n- path: /v3/tagBindings\n  method: post\n  operationId: cloudresourcemanager.tagBindings.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/cloud-platform.read-only\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/agentic-access/google-cloud-platform-agentic-access.yml
summary_line: 28 operations · 16 acting
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
---

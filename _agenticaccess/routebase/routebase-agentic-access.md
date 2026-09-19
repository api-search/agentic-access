---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 22
api_specs:
- filename: routebase-api-specs-api-openapi.yml
  format: yaml
  label: Routebase API Specs API
  slug: routebase-api-specs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routebase/refs/heads/main/openapi/routebase-api-specs-api-openapi.yml
- filename: routebase-ci-test-runs-api-openapi.yml
  format: yaml
  label: Routebase CI & Test Runs API
  slug: routebase-ci-test-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routebase/refs/heads/main/openapi/routebase-ci-test-runs-api-openapi.yml
- filename: routebase-docs-as-code-api-openapi.yml
  format: yaml
  label: Routebase Docs as Code API
  slug: routebase-docs-as-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routebase/refs/heads/main/openapi/routebase-docs-as-code-api-openapi.yml
- filename: routebase-scim-api-openapi.yml
  format: yaml
  label: Routebase SCIM API
  slug: routebase-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routebase/refs/heads/main/openapi/routebase-scim-api-openapi.yml
- filename: routebase-security-api-openapi.yml
  format: yaml
  label: Routebase Security API
  slug: routebase-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routebase/refs/heads/main/openapi/routebase-security-api-openapi.yml
consequence_counts:
  physical: 5
  read: 22
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Routebase Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/projects/{projectId}/docs/{docId}/versions/{versionId}/tree/reorder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /scim/v2/{orgSlug}/Groups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /scim/v2/{orgSlug}/Groups/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /scim/v2/{orgSlug}/Users
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /scim/v2/{orgSlug}/Users/{id}
operation_count: 37
overview: 'Routebase exposes 37 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 10 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Routebase
provider_slug: routebase
slug: routebase-agentic-access
source_filename: routebase-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: generated\nsource: openapi/routebase-public-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 22\n    acting: 15\n  by_consequence:\n    read: 22\n    write: 10\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/cli/environments\n  method: get\n  operationId: cliListEnvironments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cli/run\n  method: post\n  operationId: cliRunTestSuite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/cli/runs/{id}/report\n  method: get\n  operationId: cliDownloadReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cli/runs/{id}/status\n  method: get\n  operationId: cliGetRunStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cli/suites\n  method: get\n  operationId: cliListSuites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{projectId}/docs\n  method: get\n  operationId: getDocumentations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{projectId}/docs/{docId}/versions/{versionId}/folders\n  method: post\n  operationId: createDocFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{projectId}/docs/{docId}/versions/{versionId}/pages\n  method: post\n  operationId: createDocPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{projectId}/docs/{docId}/versions/{versionId}/pages/{pageId}\n  method: get\n  operationId: getDocPageDetail\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{projectId}/docs/{docId}/versions/{versionId}/pages/{pageId}\n  method: put\n  operationId: updateDocPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{projectId}/docs/{docId}/versions/{versionId}/tree\n  method: get\n  operationId: getDocTree\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{projectId}/docs/{docId}/versions/{versionId}/tree/reorder\n  method: put\n  operationId: reorderTreeItems\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{projectId}/security/findings\n  method: get\n  operationId: getSecurityFindings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{projectId}/security/findings/export/sarif\n  method: get\n  operationId: exportSecurityFindingsSarif\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{projectId}/security/scan-profiles/{profileId}/run\n  method: post\n  operationId: enqueueScanRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{projectId}/security/scan-runs/{runId}\n  method: get\n  operationId: getScanRunById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{projectId}/specs\n  method: get\n  operationId: getApiSpecs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{projectId}/specs/{specId}/export\n  method: get\n  operationId: exportApiSpec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{projectId}/specs/{specId}/versions\n  method: get\n  operationId: getSpecVersions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{projectId}/specs/{specId}/versions/{versionId}/export\n  method: get\n  operationId: exportSpecVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{projectId}/specs/{specId}/versions/{versionId}/promote\n  method: post\n  operationId: promoteSpecVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{projectId}/test-suites\n  method: get\n  operationId: getTestSuites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{projectId}/test-suites/{suiteId}/execute\n  method: post\n  operationId: executeTestSuite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/{orgSlug}/Groups\n  method: get\n  operationId: scimListGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/{orgSlug}/Groups\n  method: post\n  operationId: scimCreateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/{orgSlug}/Groups/{id}\n  method: get\n  operationId: scimGetGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/{orgSlug}/Groups/{id}\n  method: patch\n  operationId: scimPatchGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/{orgSlug}/Groups/{id}\n  method: delete\n  operationId: scimDeleteGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/{orgSlug}/ResourceTypes\n  method: get\n  operationId: scimResourceTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/{orgSlug}/Schemas\n  method: get\n  operationId: scimSchemas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/{orgSlug}/ServiceProviderConfig\n  method: get\n  operationId: scimServiceProviderConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/{orgSlug}/Users\n  method: get\n  operationId: scimListUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/{orgSlug}/Users\n  method: post\n  operationId: scimCreateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/{orgSlug}/Users/{id}\n  method: get\n  operationId: scimGetUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/{orgSlug}/Users/{id}\n  method: put\n  operationId: scimReplaceUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/{orgSlug}/Users/{id}\n  method: patch\n  operationId: scimPatchUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/{orgSlug}/Users/{id}\n  method: delete\n  operationId: scimDeleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/routebase/refs/heads/main/agentic-access/routebase-agentic-access.yml
summary_line: 37 operations · 15 acting
tags:
- API lifecycle management
- API Design
- OpenAPI
- API Documentation
- API Testing
- API Mocking
- API Monitoring
- API Security
- MCP
- AI Agents
- Developer Tools
- CI/CD
- REST
- OAuth 2.1
- SCIM
- Streamable HTTP
---

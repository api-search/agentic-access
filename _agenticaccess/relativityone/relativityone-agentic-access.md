---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 4
api_specs:
- filename: relativityone-legal-hold-openapi.yml
  format: yaml
  label: Legal Hold API
  slug: legal-hold-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativityone/refs/heads/main/openapi/relativityone-legal-hold-openapi.yml
consequence_counts:
  read: 4
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Relativityone Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'RelativityOne exposes 13 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: RelativityOne
provider_slug: relativityone
slug: relativityone-agentic-access
source_filename: relativityone-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/relativityone-legal-hold-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 4\n    acting: 9\n  by_consequence:\n    read: 4\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /relativity-environment/v1/workspaces/{workspaceId}/legal-hold/projects\n  method: get\n  operationId: listLegalHoldProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-environment/v1/workspaces/{workspaceId}/legal-hold/projects\n  method: post\n  operationId: createLegalHoldProject\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-environment/v1/workspaces/{workspaceId}/legal-hold/projects/{projectId}\n  method: get\n  operationId: getLegalHoldProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-environment/v1/workspaces/{workspaceId}/legal-hold/projects/{projectId}/custodians\n  method: get\n  operationId: listProjectCustodians\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-environment/v1/workspaces/{workspaceId}/legal-hold/projects/{projectId}/custodians\n  method: post\n  operationId: addCustodianToProject\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-environment/v1/workspaces/{workspaceId}/legal-hold/active-custodians\n  method: get\n  operationId: getActiveCustodianSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-environment/v1/workspaces/{workspaceId}/legal-hold/entities\n  method: post\n  operationId: createEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-environment/v1/workspaces/{workspaceId}/legal-hold/entities/{entityId}\n\
  \  method: put\n  operationId: updateEntityStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-environment/v1/workspaces/{workspaceId}/legal-hold/projects/{projectId}/preserve\n  method: post\n  operationId: preserveCustodianData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-environment/v1/workspaces/{workspaceId}/legal-hold/projects/{projectId}/release\n  method: post\n  operationId: releaseCustodianFromProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-environment/v1/workspaces/{workspaceId}/legal-hold/projects/{projectId}/communications\n  method: post\n  operationId: createLegalHoldCommunication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-environment/v1/workspaces/{workspaceId}/legal-hold/tasks\n  method: post\n  operationId: createLegalHoldTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /relativity-environment/v1/workspaces/{workspaceId}/legal-hold/tasks/{taskId}\n  method: put\n  operationId: updateLegalHoldTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relativityone/refs/heads/main/agentic-access/relativityone-agentic-access.yml
summary_line: 13 operations · 9 acting
tags:
- eDiscovery
- Legal
- Legal Hold
- Document Management
- Compliance
- Litigation
---

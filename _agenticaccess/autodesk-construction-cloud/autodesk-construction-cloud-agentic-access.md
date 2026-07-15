---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 8
api_specs:
- filename: acc-admin-openapi.yml
  format: yaml
  label: Autodesk Construction Cloud Admin API
  slug: acc-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk-construction-cloud/refs/heads/main/openapi/acc-admin-openapi.yml
- filename: acc-issues-openapi.yml
  format: yaml
  label: Autodesk Construction Cloud Issues API
  slug: acc-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk-construction-cloud/refs/heads/main/openapi/acc-issues-openapi.yml
consequence_counts:
  read: 8
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Autodesk Construction Cloud Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Autodesk Construction Cloud exposes 13 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Autodesk Construction Cloud
provider_slug: autodesk-construction-cloud
slug: autodesk-construction-cloud-agentic-access
source_filename: autodesk-construction-cloud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/acc-admin-openapi.yml, openapi/acc-issues-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 8\n    acting: 5\n  by_consequence:\n    read: 8\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /construction/admin/v1/accounts/{accountId}/projects\n  method: get\n  operationId: getAccountProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /construction/admin/v1/accounts/{accountId}/projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /construction/admin/v1/accounts/{accountId}/projects/{projectId}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /construction/admin/v1/accounts/{accountId}/projects/{projectId}\n  method: patch\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /construction/admin/v1/accounts/{accountId}/projects/{projectId}/users\n  method: get\n  operationId: getProjectUsers\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /construction/admin/v1/accounts/{accountId}/projects/{projectId}/users\n  method: post\n  operationId: addProjectUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /construction/admin/v1/accounts/{accountId}/users\n  method: get\n  operationId: getAccountUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /construction/admin/v1/accounts/{accountId}/companies\n  method: get\n  operationId: getAccountCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /issues/v2/containers/{containerId}/issues\n  method: get\n  operationId: listIssues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issues/v2/containers/{containerId}/issues\n  method: post\n  operationId: createIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issues/v2/containers/{containerId}/issues/{issueId}\n  method: get\n  operationId: getIssue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issues/v2/containers/{containerId}/issues/{issueId}\n  method: patch\n  operationId: updateIssue\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issues/v2/containers/{containerId}/issue-types\n  method: get\n  operationId: listIssueTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autodesk-construction-cloud/refs/heads/main/agentic-access/autodesk-construction-cloud-agentic-access.yml
summary_line: 13 operations · 5 acting
tags:
- Construction
- BIM
- Project Management
- AEC
- CAD
- Architecture
- Engineering
- Field Management
---

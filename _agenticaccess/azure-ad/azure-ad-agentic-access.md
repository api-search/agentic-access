---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 10
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph API
  slug: microsoft-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
consequence_counts:
  read: 10
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Azure Ad Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Azure Active Directory exposes 14 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Azure Active Directory
provider_slug: azure-ad
slug: azure-ad-agentic-access
source_filename: azure-ad-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/azure-ad-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 10\n    acting: 4\n  by_consequence:\n    read: 10\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - User.Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/photo/$value\n  method: get\n  operationId: getMyPhoto\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - User.Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - User.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - User.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - User.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}\n  method: patch\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - User.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - User.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}/manager\n  method: get\n  operationId: getUserManager\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - User.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}/directReports\n  method: get\n  operationId: listDirectReports\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - User.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Group.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups\n  method: post\n  operationId: createGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Group.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{id}\n  method: get\n  operationId: getGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Group.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications\n  method:\
  \ get\n  operationId: listApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Application.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /directoryRoles\n  method: get\n  operationId: listDirectoryRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Directory.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/agentic-access/azure-ad-agentic-access.yml
summary_line: 14 operations · 4 acting
tags:
- Authentication
- Authorization
- Identity
- OAuth
- OpenID Connect
- Single Sign-On
---

---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 14
api_specs:
- filename: active-directory-users-openapi.yaml
  format: yaml
  label: Microsoft Graph Users API
  slug: microsoft-graph-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/openapi/active-directory-users-openapi.yaml
- filename: active-directory-groups-openapi.yaml
  format: yaml
  label: Microsoft Graph Groups API
  slug: microsoft-graph-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/openapi/active-directory-groups-openapi.yaml
- filename: active-directory-applications-openapi.yaml
  format: yaml
  label: Microsoft Graph Applications and Service Principals API
  slug: microsoft-graph-applications-and-service-principals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/openapi/active-directory-applications-openapi.yaml
consequence_counts:
  read: 14
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Active Directory Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Microsoft Active Directory exposes 25 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Active Directory
provider_slug: active-directory
slug: active-directory-agentic-access
source_filename: active-directory-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/active-directory-applications-openapi.yaml, openapi/active-directory-groups-openapi.yaml,\n  openapi/active-directory-users-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 14\n    acting: 11\n  by_consequence:\n    read: 14\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /applications\n  method: get\n  operationId: list-applications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Application.Read.All\n    - Application.ReadWrite.All\n- path: /applications\n  method: post\n  operationId: create-application\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Application.Read.All\n    - Application.ReadWrite.All\n- path: /applications/{applicationId}\n  method: get\n  operationId: get-application\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Application.Read.All\n    - Application.ReadWrite.All\n- path: /applications/{applicationId}\n  method: patch\n  operationId: update-application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n    scope:\n    - Application.Read.All\n    - Application.ReadWrite.All\n- path: /applications/{applicationId}\n  method: delete\n  operationId: delete-application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Application.Read.All\n    - Application.ReadWrite.All\n- path: /servicePrincipals\n  method: get\n  operationId: list-service-principals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Application.Read.All\n    - Application.ReadWrite.All\n- path: /servicePrincipals/{servicePrincipalId}\n  method: get\n  operationId: get-service-principal\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Application.Read.All\n    - Application.ReadWrite.All\n- path: /servicePrincipals/{servicePrincipalId}/appRoleAssignments\n  method: get\n  operationId: list-service-principal-app-role-assignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Application.Read.All\n    - Application.ReadWrite.All\n- path: /groups\n  method: get\n  operationId: list-groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n- path: /groups\n  method: post\n  operationId: create-group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n- path: /groups/{groupId}\n  method: get\n  operationId: get-group\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n- path: /groups/{groupId}\n  method: patch\n  operationId: update-group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n- path: /groups/{groupId}\n  method: delete\n  operationId: delete-group\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n- path: /groups/{groupId}/members\n  method: get\n  operationId: list-group-members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n- path: /groups/{groupId}/members\n  method: post\n  operationId: add-group-member\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n- path: /groups/{groupId}/members/{memberId}/$ref\n\
  \  method: delete\n  operationId: remove-group-member\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n- path: /groups/{groupId}/owners\n  method: get\n  operationId: list-group-owners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n- path: /users\n  method: get\n  operationId: list-users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - User.Read\n    - User.Read.All\n    - User.ReadBasic.All\n    - User.ReadWrite\n    - User.ReadWrite.All\n\
  - path: /users\n  method: post\n  operationId: create-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - User.Read\n    - User.Read.All\n    - User.ReadBasic.All\n    - User.ReadWrite\n    - User.ReadWrite.All\n- path: /users/{userId}\n  method: get\n  operationId: get-user\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - User.Read\n    - User.Read.All\n    - User.ReadBasic.All\n    - User.ReadWrite\n    - User.ReadWrite.All\n- path: /users/{userId}\n  method: patch\n  operationId: update-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - User.Read\n    - User.Read.All\n    - User.ReadBasic.All\n    - User.ReadWrite\n    - User.ReadWrite.All\n- path: /users/{userId}\n  method: delete\n  operationId: delete-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - User.Read\n    - User.Read.All\n    - User.ReadBasic.All\n    - User.ReadWrite\n    - User.ReadWrite.All\n- path: /users/{userId}/memberOf\n  method: get\n  operationId: list-user-member-of\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - User.Read\n    -\
  \ User.Read.All\n    - User.ReadBasic.All\n    - User.ReadWrite\n    - User.ReadWrite.All\n- path: /users/{userId}/manager\n  method: get\n  operationId: get-user-manager\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - User.Read\n    - User.Read.All\n    - User.ReadBasic.All\n    - User.ReadWrite\n    - User.ReadWrite.All\n- path: /me\n  method: get\n  operationId: get-me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - User.Read\n    - User.Read.All\n    - User.ReadBasic.All\n    - User.ReadWrite\n    - User.ReadWrite.All\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/agentic-access/active-directory-agentic-access.yml
summary_line: 25 operations · 11 acting
tags:
- Active Directory
- Authentication
- Authorization
- Directory Services
- Identity Management
- Microsoft Entra
- Zero Trust
---

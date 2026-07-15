---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 11
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph API
  slug: microsoft-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: microsoft-graph-identity-api.yml
  format: yaml
  label: Microsoft Graph Identity and Access API
  slug: microsoft-graph-identity-and-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/openapi/microsoft-graph-identity-api.yml
consequence_counts:
  read: 11
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Azure Active Directory Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'Microsoft Azure Active Directory exposes 24 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Azure Active Directory
provider_slug: microsoft-azure-active-directory
slug: microsoft-azure-active-directory-agentic-access
source_filename: microsoft-azure-active-directory-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-graph-identity-api.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 11\n    acting: 13\n  by_consequence:\n    read: 11\n    write: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Directory.Read.All\n    - User.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Directory.ReadWrite.All\n\
  \    - User.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user-id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Directory.Read.All\n    - User.Read\n    - User.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user-id}\n  method: patch\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Directory.ReadWrite.All\n    - User.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user-id}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Directory.ReadWrite.All\n    - User.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user-id}/memberOf\n  method: get\n  operationId: listUserMemberOf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Directory.Read.All\n    - User.Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Directory.Read.All\n    - Group.Read.All\n    - GroupMember.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups\n  method: post\n  operationId: createGroup\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - Directory.ReadWrite.All\n    - Group.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group-id}\n  method: get\n  operationId: getGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Directory.Read.All\n    - Group.Read.All\n    - GroupMember.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group-id}\n  method: patch\n  operationId: updateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Directory.ReadWrite.All\n    - Group.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /groups/{group-id}\n  method: delete\n  operationId: deleteGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Directory.ReadWrite.All\n    - Group.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group-id}/members\n  method: get\n  operationId: listGroupMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Directory.Read.All\n    - Group.Read.All\n    - GroupMember.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group-id}/members/$ref\n  method: post\n  operationId: addGroupMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Directory.ReadWrite.All\n    - Group.ReadWrite.All\n\
  \    - GroupMember.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications\n  method: get\n  operationId: listApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Application.Read.All\n    - Directory.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications\n  method: post\n  operationId: createApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Application.ReadWrite.All\n    - Directory.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-id}\n  method: get\n  operationId: getApplication\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Application.Read.All\n    - Directory.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-id}\n  method: patch\n  operationId: updateApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Application.ReadWrite.All\n    - Directory.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-id}\n  method: delete\n  operationId: deleteApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Application.ReadWrite.All\n    - Directory.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servicePrincipals\n  method: get\n  operationId: listServicePrincipals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Application.Read.All\n    - Directory.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servicePrincipals\n  method: post\n  operationId: createServicePrincipal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Application.ReadWrite.All\n    - Directory.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servicePrincipals/{servicePrincipal-id}\n  method: get\n  operationId: getServicePrincipal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - Application.Read.All\n    - Directory.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servicePrincipals/{servicePrincipal-id}\n  method: patch\n  operationId: updateServicePrincipal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Application.ReadWrite.All\n    - Directory.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servicePrincipals/{servicePrincipal-id}\n  method: delete\n  operationId: deleteServicePrincipal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Application.ReadWrite.All\n    - Directory.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /servicePrincipals/{servicePrincipal-id}/appRoleAssignments\n  method: get\n  operationId: listServicePrincipalAppRoleAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Application.Read.All\n    - Directory.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/agentic-access/microsoft-azure-active-directory-agentic-access.yml
summary_line: 24 operations · 13 acting
tags:
- Authentication
- Authorization
- Identity
- Microsoft
- Microsoft Entra
- OAuth
- OpenID Connect
- SAML
- SCIM
- Single Sign-On
- Zero Trust
---

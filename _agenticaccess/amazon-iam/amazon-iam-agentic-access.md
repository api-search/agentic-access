---
acting_count: 0
action_class_counts:
  connected: 25
api_specs:
- filename: amazon-iam-openapi.yml
  format: yaml
  label: AWS IAM API
  slug: aws-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/openapi/amazon-iam-openapi.yml
consequence_counts:
  read: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Iam Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Amazon IAM exposes 25 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon IAM
provider_slug: amazon-iam
slug: amazon-iam-agentic-access
source_filename: amazon-iam-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-iam-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 25\n  by_consequence:\n    read: 25\n  human_in_the_loop_required: 0\noperations:\n- path: /?Action=CreateUser\n  method: get\n  operationId: CreateUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=GetUser\n  method: get\n  operationId: GetUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=ListUsers\n  method: get\n  operationId: ListUsers\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=UpdateUser\n  method: get\n  operationId: UpdateUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DeleteUser\n  method: get\n  operationId: DeleteUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=CreateRole\n  method: get\n  operationId: CreateRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=GetRole\n  method: get\n  operationId: GetRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /?Action=ListRoles\n  method: get\n  operationId: ListRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DeleteRole\n  method: get\n  operationId: DeleteRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=AssumeRole\n  method: get\n  operationId: AssumeRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=CreatePolicy\n  method: get\n  operationId: CreatePolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=GetPolicy\n  method: get\n  operationId: GetPolicy\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=ListPolicies\n  method: get\n  operationId: ListPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=AttachUserPolicy\n  method: get\n  operationId: AttachUserPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=AttachRolePolicy\n  method: get\n  operationId: AttachRolePolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DetachUserPolicy\n  method: get\n  operationId: DetachUserPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /?Action=DetachRolePolicy\n  method: get\n  operationId: DetachRolePolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=CreateGroup\n  method: get\n  operationId: CreateGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=GetGroup\n  method: get\n  operationId: GetGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=ListGroups\n  method: get\n  operationId: ListGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=AddUserToGroup\n  method: get\n  operationId: AddUserToGroup\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=RemoveUserFromGroup\n  method: get\n  operationId: RemoveUserFromGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=CreateAccessKey\n  method: get\n  operationId: CreateAccessKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=ListAccessKeys\n  method: get\n  operationId: ListAccessKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DeleteAccessKey\n  method: get\n  operationId: DeleteAccessKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/agentic-access/amazon-iam-agentic-access.yml
summary_line: 25 operations
tags:
- Access Management
- Authentication
- Authorization
- Identity
- Security
---

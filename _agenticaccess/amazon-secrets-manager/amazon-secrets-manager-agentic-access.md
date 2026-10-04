---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 2
api_specs:
- filename: amazon-secrets-manager-passwords-api-openapi.yml
  format: yaml
  label: Amazon Secrets Manager Passwords API
  slug: amazon-secrets-manager-passwords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/openapi/amazon-secrets-manager-passwords-api-openapi.yml
- filename: amazon-secrets-manager-rotation-api-openapi.yml
  format: yaml
  label: Amazon Secrets Manager Rotation API
  slug: amazon-secrets-manager-rotation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/openapi/amazon-secrets-manager-rotation-api-openapi.yml
- filename: amazon-secrets-manager-secrets-api-openapi.yml
  format: yaml
  label: Amazon Secrets Manager Secrets API
  slug: amazon-secrets-manager-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/openapi/amazon-secrets-manager-secrets-api-openapi.yml
- filename: amazon-secrets-manager-amazon-secrets-manager-api-api-openapi.yml
  format: yaml
  label: Amazon Secrets Manager Amazon Secrets Manager API
  slug: amazon-secrets-manager-amazon-secrets-manager-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/openapi/amazon-secrets-manager-amazon-secrets-manager-api-api-openapi.yml
consequence_counts:
  read: 2
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Secrets Manager Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Amazon Secrets Manager exposes 12 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Secrets Manager
provider_slug: amazon-secrets-manager
slug: amazon-secrets-manager-agentic-access
source_filename: amazon-secrets-manager-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/amazon-secrets-manager-passwords-api-openapi.yml, openapi/amazon-secrets-manager-rotation-api-openapi.yml,\n  openapi/amazon-secrets-manager-secrets-api-openapi.yml, openapi/amazon-secrets-manager-tag-resource-api-openapi.yml,\n  openapi/amazon-secrets-manager-untag-resource-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 10\n    connected: 2\n  by_consequence:\n    write: 10\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /#GetRandomPassword\n  method: post\n  operationId: GetRandomPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#RotateSecret\n  method: post\n  operationId: RotateSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: post\n  operationId: CreateSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#GetSecretValue\n  method: post\n  operationId: GetSecretValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /#PutSecretValue\n  method: post\n  operationId: PutSecretValue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#UpdateSecret\n  method: post\n  operationId: UpdateSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DeleteSecret\n  method: post\n  operationId: DeleteSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#ListSecrets\n  method: post\n  operationId: ListSecrets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#DescribeSecret\n  method: post\n  operationId: DescribeSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#RestoreSecret\n  method: post\n  operationId: RestoreSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /#TagResource\n  method: post\n  operationId: TagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#UntagResource\n  method: post\n  operationId: UntagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/agentic-access/amazon-secrets-manager-agentic-access.yml
summary_line: 12 operations · 10 acting
tags:
- Configuration
- Credentials
- Rotation
- Secrets
- Security
---

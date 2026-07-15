---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 4
api_specs:
- filename: azure-management-openapi.yaml
  format: yaml
  label: Azure Compute API
  slug: azure-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/openapi/azure-management-openapi.yaml
- filename: azure-management-openapi.yaml
  format: yaml
  label: Azure Storage API
  slug: azure-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/openapi/azure-management-openapi.yaml
- filename: azure-management-openapi.yaml
  format: yaml
  label: Azure Cognitive Services API
  slug: azure-cognitive-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/openapi/azure-management-openapi.yaml
consequence_counts:
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Azure Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Microsoft Azure exposes 5 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Azure
provider_slug: azure
slug: azure-agentic-access
source_filename: azure-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/azure-management-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 4\n    acting: 1\n  by_consequence:\n    read: 4\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /subscriptions\n  method: get\n  operationId: Subscriptions_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}\n  method: get\n  operationId: Subscriptions_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups\n  method: get\n  operationId: ResourceGroups_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups\n  method: post\n  operationId: ResourceGroups_CreateOrUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resources\n  method: get\n  operationId: Resources_ListBySubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/agentic-access/azure-agentic-access.yml
summary_line: 5 operations · 1 acting
tags:
- Cloud Computing
- Databases
- Infrastructure
- Machine Learning
- Networking
- Platform as a Service
- Storage
---

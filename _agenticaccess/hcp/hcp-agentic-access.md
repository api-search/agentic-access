---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 7
api_specs:
- filename: hcp-openapi.yml
  format: yaml
  label: HCP Vault Secrets API
  slug: hcp-vault-secrets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hcp/refs/heads/main/openapi/hcp-openapi.yml
consequence_counts:
  read: 7
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hcp Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'HashiCorp Cloud Platform exposes 9 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HashiCorp Cloud Platform
provider_slug: hcp
slug: hcp-agentic-access
source_filename: hcp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hcp-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 7\n    acting: 2\n  by_consequence:\n    read: 7\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /secrets/2023-11-28/organizations/{org_id}/projects/{project_id}/apps\n  method: get\n  operationId: listApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /secrets/2023-11-28/organizations/{org_id}/projects/{project_id}/apps\n  method: post\n  operationId: createApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /secrets/2023-11-28/organizations/{org_id}/projects/{project_id}/apps/{app_name}/secrets\n  method: get\n  operationId: listSecrets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /secrets/2023-11-28/organizations/{org_id}/projects/{project_id}/apps/{app_name}/secrets/{name}\n  method: get\n  operationId: getSecret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /secrets/2023-11-28/organizations/{org_id}/projects/{project_id}/apps/{app_name}/secrets/{name}\n  method: delete\n  operationId: deleteSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /secrets/2023-11-28/organizations/{org_id}/projects/{project_id}/apps/{app_name}/secrets/{name}:open\n  method: get\n  operationId: openSecret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /secrets/2023-11-28/organizations/{org_id}/projects/{project_id}/integrations\n  method: get\n  operationId: listIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /secrets/2023-11-28/organizations/{org_id}/projects/{project_id}/syncs\n  method: get\n  operationId: listSyncs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /secrets/2023-11-28/organizations/{org_id}/projects/{project_id}/gateway-pools\n  method: get\n  operationId: listGatewayPools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hcp/refs/heads/main/agentic-access/hcp-agentic-access.yml
summary_line: 9 operations · 2 acting
tags:
- Cloud
- Infrastructure
- DevOps
- Secrets Management
- Service Networking
- Fortune 1000
---

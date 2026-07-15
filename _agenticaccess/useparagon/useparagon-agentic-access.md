---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 7
api_specs:
- filename: useparagon-openapi.yml
  format: yaml
  label: Paragon Connect API
  slug: paragon-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-openapi.yml
- filename: useparagon-openapi.yml
  format: yaml
  label: Paragon Integrations API
  slug: paragon-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-openapi.yml
- filename: useparagon-openapi.yml
  format: yaml
  label: Paragon Users API
  slug: paragon-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-openapi.yml
- filename: useparagon-openapi.yml
  format: yaml
  label: Paragon Workflows API
  slug: paragon-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-openapi.yml
- filename: useparagon-openapi.yml
  format: yaml
  label: Paragon Proxy API
  slug: paragon-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-openapi.yml
- filename: useparagon-openapi.yml
  format: yaml
  label: Paragon ActionKit API
  slug: paragon-actionkit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-openapi.yml
- filename: useparagon-openapi.yml
  format: yaml
  label: Paragon Managed Sync API
  slug: paragon-managed-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-openapi.yml
- filename: useparagon-openapi.yml
  format: yaml
  label: Paragon Permissions API
  slug: paragon-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-openapi.yml
- filename: useparagon-openapi.yml
  format: yaml
  label: Paragon Events and Webhooks API
  slug: paragon-events-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-openapi.yml
consequence_counts:
  read: 7
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Useparagon Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Paragon exposes 13 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Paragon
provider_slug: useparagon
slug: useparagon-agentic-access
source_filename: useparagon-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/useparagon-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 7\n    acting: 6\n  by_consequence:\n    read: 7\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /projects/{projectId}/sdk/me\n  method: get\n  operationId: getAuthenticatedUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/sdk/integrations\n  method: get\n  operationId: listIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /projects/{projectId}/sdk/resources/{resourceId}/connect\n  method: post\n  operationId: connectResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/sdk/triggers/{workflowId}\n  method: post\n  operationId: triggerWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/sdk/workflows/{workflowId}/executions/{executionId}\n  method: get\n  operationId: getWorkflowExecution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/sdk/proxy/{integrationType}/{apiPath}\n  method: post\n  operationId: proxyRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/actions\n  method: get\n  operationId: listActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/actions/run\n  method: post\n  operationId: runAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/syncs\n  method: post\n  operationId: createSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/syncs\n  method: get\n  operationId: listSyncs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sync/{syncId}/records\n  method: get\n  operationId: listSyncRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sync/{syncId}/records/{recordId}/content\n  method: get\n  operationId: getRecordContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /permissions/check\n  method: post\n  operationId: checkPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/agentic-access/useparagon-agentic-access.yml
summary_line: 13 operations · 6 acting
tags:
- Integration
- iPaaS
- Embedded Integrations
- Workflows
- ActionKit
- Managed Sync
- AI Agents
---

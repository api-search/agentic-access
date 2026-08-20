---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 13
api_specs:
- filename: abloatai-branches-api-openapi.yml
  format: yaml
  label: Ablo Branches API
  slug: ablo-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-branches-api-openapi.yml
- filename: abloatai-claims-api-openapi.yml
  format: yaml
  label: Ablo Claims API
  slug: ablo-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-claims-api-openapi.yml
- filename: abloatai-commits-api-openapi.yml
  format: yaml
  label: Ablo Commits API
  slug: ablo-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-commits-api-openapi.yml
- filename: abloatai-credentials-api-openapi.yml
  format: yaml
  label: Ablo Credentials API
  slug: ablo-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-credentials-api-openapi.yml
- filename: abloatai-logs-api-openapi.yml
  format: yaml
  label: Ablo Logs API
  slug: ablo-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-logs-api-openapi.yml
- filename: abloatai-models-api-openapi.yml
  format: yaml
  label: Ablo Models API
  slug: ablo-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-models-api-openapi.yml
- filename: abloatai-schema-api-openapi.yml
  format: yaml
  label: Ablo Schema API
  slug: ablo-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-schema-api-openapi.yml
consequence_counts:
  physical: 1
  read: 13
  safety-critical: 2
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Abloatai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/branches/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/capabilities/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/models/{model}/{id}/claim/reorder
operation_count: 32
overview: 'Ablo exposes 32 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 16 write, 1 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ablo
provider_slug: abloatai
slug: abloatai-agentic-access
source_filename: abloatai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: generated\nsource: openapi/abloatai-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 13\n    acting: 19\n  by_consequence:\n    read: 13\n    write: 16\n    physical: 1\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v1/models/{model}\n  method: get\n  operationId: listModelRows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/models/{model}\n  method: post\n  operationId: createModelRow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models/{model}/{id}\n  method: get\n  operationId: getModelRow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/models/{model}/{id}\n  method: patch\n  operationId: updateModelRow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models/{model}/{id}\n  method: delete\n  operationId: deleteModelRow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models/{model}/{id}/claim\n  method: post\n  operationId: acquireModelClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models/{model}/{id}/claim\n  method: delete\n  operationId: releaseModelClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models/{model}/{id}/claim/heartbeat\n  method: post\n  operationId: heartbeatModelClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models/{model}/{id}/claim/reorder\n  method: post\n  operationId: reorderModelClaimQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ephemeral_keys\n  method: post\n  operationId: mintEphemeralKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/branches\n  method:\
  \ get\n  operationId: listBranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/branches\n  method: post\n  operationId: createBranch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/branches/{id}\n  method: get\n  operationId: getBranch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/branches/{id}\n  method: delete\n  operationId: deleteBranch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/branches/{id}/credentials\n  method: post\n  operationId: mintBranchCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/branches/{id}/status\n  method: get\n  operationId: getBranchStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/claims\n  method: get\n  operationId: listClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/claims\n  method: post\n  operationId: acquireClaim\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/claims/heartbeat\n  method: post\n  operationId: heartbeatClaims\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/claims/{claimId}\n  method: get\n  operationId: getClaim\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/claims/{claimId}\n  method: delete\n  operationId: releaseClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/claims/{claimId}/heartbeat\n  method: post\n  operationId: heartbeatClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/capabilities\n  method: post\n  operationId: mintCapability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/capabilities/{id}\n  method: get\n  operationId: getCapability\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/capabilities/{id}\n  method: delete\n  operationId: revokeCapability\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/capabilities/{id}/rotate\n  method: post\n  operationId: rotateCapability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/schema\n  method: get\n  operationId: getSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/logs\n  method: get\n  operationId: listLogEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/logs/delivery\n  method: get\n  operationId: getLogDelivery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/commits\n  method: get\n  operationId: listCommits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/commits\n  method: post\n  operationId: commit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/commits/{id}\n  method: get\n  operationId: getCommit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/agentic-access/abloatai-agentic-access.yml
summary_line: 32 operations · 19 acting · 2 human-in-the-loop
tags:
- Agent Infrastructure
- multi-agent-coordination
- concurrency-control
- State Management
- Database
- Postgres
- real-time-sync
- MCP
- Developer Tools
- backend-infrastructure
---

---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 12
api_specs:
- filename: bubblio-dev-agent-keys-api-openapi.yml
  format: yaml
  label: bubblio-dev Agent Keys API
  slug: bubblio-dev-agent-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bubblio-dev/openapi/bubblio-dev-agent-keys-api-openapi.yml
- filename: bubblio-dev-approvals-api-openapi.yml
  format: yaml
  label: bubblio-dev Approvals API
  slug: bubblio-dev-approvals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bubblio-dev/openapi/bubblio-dev-approvals-api-openapi.yml
- filename: bubblio-dev-discovery-api-openapi.yml
  format: yaml
  label: bubblio-dev Discovery API
  slug: bubblio-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bubblio-dev/openapi/bubblio-dev-discovery-api-openapi.yml
- filename: bubblio-dev-mcp-api-openapi.yml
  format: yaml
  label: bubblio-dev MCP API
  slug: bubblio-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bubblio-dev/openapi/bubblio-dev-mcp-api-openapi.yml
- filename: bubblio-dev-platform-push-api-openapi.yml
  format: yaml
  label: bubblio-dev Platform Push API
  slug: bubblio-dev-platform-push-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bubblio-dev/openapi/bubblio-dev-platform-push-api-openapi.yml
- filename: bubblio-dev-platform-sync-api-openapi.yml
  format: yaml
  label: bubblio-dev Platform Sync API
  slug: bubblio-dev-platform-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bubblio-dev/openapi/bubblio-dev-platform-sync-api-openapi.yml
consequence_counts:
  physical: 1
  read: 12
  safety-critical: 3
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Bubblio Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /approvals/mine/mandates/{mandateId}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /approvals/mine/{approvalId}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/agent-keys/{keyId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/agent-door/paid/{quoteId}
operation_count: 27
overview: 'bubblio-dev exposes 27 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 11 write, 1 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: bubblio-dev
provider_slug: bubblio-dev
slug: bubblio-dev-agentic-access
source_filename: bubblio-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/bubblio-dev-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 12\n    acting: 15\n  by_consequence:\n    read: 12\n    write: 11\n    safety-critical: 3\n    physical: 1\n  human_in_the_loop_required: 3\noperations:\n- path: /agent/directory\n  method: get\n  operationId: getDirectory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/feed.json\n  method: get\n  operationId: getAgentFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /agent/resolve\n  method: get\n  operationId: resolveDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/hub\n  method: get\n  operationId: getHubManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/hub/llms.txt\n  method: get\n  operationId: getHubLlmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/hub/mcp\n  method: get\n  operationId: getHubMcp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/hub/mcp\n  method: post\n  operationId: postHubMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/{doorId}\n  method: get\n  operationId: getDoorManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/{doorId}/llms.txt\n  method: get\n  operationId: getDoorLlmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/{doorId}/mcp\n  method: get\n  operationId: getDoorMcp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/{doorId}/mcp\n  method: post\n  operationId: postDoorMcp\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /approvals/a/{approvalId}\n  method: get\n  operationId: getApproval\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /approvals/a/{approvalId}/options\n  method: post\n  operationId: postApprovalOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /approvals/a/{approvalId}/approve\n  method: post\n  operationId: postApprovalApprove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /approvals/a/{approvalId}/decline\n  method: post\n  operationId: postApprovalDecline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /approvals/session/options\n  method: post\n  operationId: postSessionOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /approvals/session\n  method: post\n  operationId: postSession\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /approvals/mine\n  method: get\n  operationId: getMine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /approvals/mine/{approvalId}/revoke\n  method: post\n  operationId: postRevokeApproval\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /approvals/mine/mandates/{mandateId}/revoke\n  method: post\n  operationId: postRevokeMandate\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/agent-keys\n  method: post\n  operationId: mintAgentKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent-keys\n  method: get\n  operationId: listAgentKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent-keys/{keyId}\n  method: delete\n  operationId: revokeAgentKey\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/agent-keys/connect-grant\n  method: post\n  operationId: postConnectGrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent-door/actions/sync\n  method: post\n  operationId: syncDoorActions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent-door/results/{quoteId}\n\
  \  method: post\n  operationId: pushDoorResult\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent-door/paid/{quoteId}\n  method: post\n  operationId: resumePaidQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/bubblio-dev/agentic-access/bubblio-dev-agentic-access.yml
summary_line: 27 operations · 15 acting · 3 human-in-the-loop
tags:
- Artificial Intelligence
- Payments
- Automation
- Platform
- Agents
---

---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 15
api_specs:
- filename: axiorank-com-audit-api-openapi.yml
  format: yaml
  label: AxioRank Audit API
  slug: axiorank-com-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiorank-com/openapi/axiorank-com-audit-api-openapi.yml
- filename: axiorank-com-gateway-api-openapi.yml
  format: yaml
  label: AxioRank Gateway API
  slug: axiorank-com-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiorank-com/openapi/axiorank-com-gateway-api-openapi.yml
- filename: axiorank-com-health-api-openapi.yml
  format: yaml
  label: AxioRank Health API
  slug: axiorank-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiorank-com/openapi/axiorank-com-health-api-openapi.yml
- filename: axiorank-com-mcp-api-openapi.yml
  format: yaml
  label: AxioRank MCP API
  slug: axiorank-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiorank-com/openapi/axiorank-com-mcp-api-openapi.yml
- filename: axiorank-com-protocols-api-openapi.yml
  format: yaml
  label: AxioRank Protocols API
  slug: axiorank-com-protocols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiorank-com/openapi/axiorank-com-protocols-api-openapi.yml
- filename: axiorank-com-tools-log-api-openapi.yml
  format: yaml
  label: AxioRank Tools Log API
  slug: axiorank-com-tools-log-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiorank-com/openapi/axiorank-com-tools-log-api-openapi.yml
consequence_counts:
  read: 15
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Axiorank Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'AxioRank exposes 22 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AxioRank
provider_slug: axiorank-com
slug: axiorank-com-agentic-access
source_filename: axiorank-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/axiorank-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 7\n    connected: 15\n  by_consequence:\n    write: 7\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/gateway/tool-call\n  method: post\n  operationId: scoreToolCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/gateway/approvals/{approvalId}\n  method: get\n  operationId: pollApproval\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/gateway/verify-card\n  method: post\n  operationId: verifyCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/gateway/verify-request\n  method: post\n  operationId: verifyRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/gateway/token\n  method: post\n  operationId: exchangeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/gateway/mcp-tool-call\n  method: post\n  operationId: evaluateMcpToolCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/audit/export\n  method: get\n  operationId: exportAuditLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/audit/public-key\n  method: get\n  operationId: auditPublicKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/audit/verify-receipt\n  method: post\n  operationId: verifyAuditReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/audit/checkpoints/{seq}\n  method: get\n  operationId: auditCheckpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/audit/receipt/{auditLogId}\n  method: get\n  operationId: auditReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/audit/log/{logId}/checkpoints\n  method: get\n  operationId: listLogCheckpoints\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/audit/log/{logId}/checkpoints/latest\n  method: get\n  operationId: latestLogCheckpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/audit/log/{logId}/checkpoints/{seq}\n  method: get\n  operationId: logCheckpointBySeq\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/protocols\n  method: get\n  operationId: protocols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/mcp/{serverId}\n  method: post\n  operationId: mcpProxy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools-log/servers\n  method: get\n  operationId: toolLogServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools-log/servers/{host}\n  method: get\n  operationId: toolLogServerHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools-log/entries/{id}\n  method: get\n  operationId: toolLogEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools-log/entries/{id}/proof\n  method: get\n  operationId: toolLogEntryProof\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools-log/sth\n  method: get\n  operationId: toolLogSth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/axiorank-com/agentic-access/axiorank-com-agentic-access.yml
summary_line: 22 operations · 7 acting
tags:
- Artificial Intelligence
- Security
- Gateways
- Zero Trust
- Agents
---

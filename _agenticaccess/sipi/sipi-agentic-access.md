---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 8
api_specs:
- filename: sipi-agents-api-openapi.yml
  format: yaml
  label: GitDealFlow Agents API
  slug: sipi-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sipi/refs/heads/main/openapi/sipi-agents-api-openapi.yml
- filename: sipi-approvals-api-openapi.yml
  format: yaml
  label: GitDealFlow Approvals API
  slug: sipi-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sipi/refs/heads/main/openapi/sipi-approvals-api-openapi.yml
- filename: sipi-budget-api-openapi.yml
  format: yaml
  label: GitDealFlow Budget API
  slug: sipi-budget-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sipi/refs/heads/main/openapi/sipi-budget-api-openapi.yml
- filename: sipi-evaluate-api-openapi.yml
  format: yaml
  label: GitDealFlow Evaluate API
  slug: sipi-evaluate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sipi/refs/heads/main/openapi/sipi-evaluate-api-openapi.yml
- filename: sipi-rules-api-openapi.yml
  format: yaml
  label: GitDealFlow Rules API
  slug: sipi-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sipi/refs/heads/main/openapi/sipi-rules-api-openapi.yml
- filename: sipi-system-api-openapi.yml
  format: yaml
  label: GitDealFlow System API
  slug: sipi-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sipi/refs/heads/main/openapi/sipi-system-api-openapi.yml
consequence_counts:
  read: 8
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sipi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'GitDealFlow exposes 13 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GitDealFlow
provider_slug: sipi
slug: sipi-agentic-access
source_filename: sipi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: generated\nsource: openapi/sipi-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 5\n    connected: 8\n  by_consequence:\n    write: 5\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/transactions/evaluate\n  method: post\n  operationId: evaluateTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rules\n  method: get\n  operationId: listRules\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rules\n  method: post\n  operationId: addRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rules/{rule_id}\n  method: delete\n  operationId: deleteRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/approvals\n  method: get\n  operationId: listApprovals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/approvals/{approval_id}\n  method: post\n  operationId: resolveApproval\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents\n  method: post\n  operationId: registerAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/status\n  method: get\n  operationId: billingStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-card.json\n  method: get\n  operationId: agentCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sipi/refs/heads/main/agentic-access/sipi-agentic-access.yml
summary_line: 13 operations · 5 acting
tags:
- Artificial Intelligence
- Finance
- Security
- Automation
- Software-as-a-Service
---

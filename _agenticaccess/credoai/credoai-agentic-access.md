---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 6
api_specs:
- filename: credoai-audit-logs-api-openapi.yml
  format: yaml
  label: Credoai Audit Logs API
  slug: credoai-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credoai/refs/heads/main/openapi/credoai-audit-logs-api-openapi.yml
- filename: credoai-shadow-ai-api-openapi.yml
  format: yaml
  label: Credoai Shadow AI API
  slug: credoai-shadow-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credoai/refs/heads/main/openapi/credoai-shadow-ai-api-openapi.yml
consequence_counts:
  read: 6
  safety-critical: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Credoai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /shadow_ai/ai_events
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /shadow_ai/ai_events/bulk
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /shadow_ai/ai_events/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /shadow_ai/ai_tools/{id}/register
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /shadow_ai/ai_tools/{id}/unregister
operation_count: 11
overview: 'Credoai exposes 11 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Credoai
provider_slug: credoai
slug: credoai-agentic-access
source_filename: credoai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: generated\nsource: openapi/credoai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 6\n    acting: 5\n  by_consequence:\n    read: 6\n    safety-critical: 5\n  human_in_the_loop_required: 5\noperations:\n- path: /audit_logs\n  method: get\n  operationId: CredoAIWeb.API.V2.AuditLogsController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit_logs/export\n  method: get\n  operationId: CredoAIWeb.API.V2.AuditLogsController.export\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /audit_logs/filter_options\n  method: get\n  operationId: CredoAIWeb.API.V2.AuditLogsController.filter_options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit_logs/{id}\n  method: get\n  operationId: CredoAIWeb.API.V2.AuditLogsController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shadow_ai/ai_events\n  method: get\n  operationId: CredoAIWeb.API.V2.ShadowAI.AIEventController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shadow_ai/ai_events\n  method: post\n  operationId: CredoAIWeb.API.V2.ShadowAI.AIEventController.create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /shadow_ai/ai_events/bulk\n  method: post\n  operationId: CredoAIWeb.API.V2.ShadowAI.AIEventController.create_bulk\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /shadow_ai/ai_events/{id}\n  method: delete\n  operationId: CredoAIWeb.API.V2.ShadowAI.AIEventController.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /shadow_ai/ai_tools\n  method: get\n  operationId: CredoAIWeb.API.V2.ShadowAI.AIToolController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shadow_ai/ai_tools/{id}/register\n  method: post\n  operationId: CredoAIWeb.API.V2.ShadowAI.AIToolController.register\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /shadow_ai/ai_tools/{id}/unregister\n  method: post\n  operationId: CredoAIWeb.API.V2.ShadowAI.AIToolController.unregister\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credoai/refs/heads/main/agentic-access/credoai-agentic-access.yml
summary_line: 11 operations · 5 acting · 5 human-in-the-loop
tags:
- Company
- AI
- Governance
- SaaS
- PaloAlto
---

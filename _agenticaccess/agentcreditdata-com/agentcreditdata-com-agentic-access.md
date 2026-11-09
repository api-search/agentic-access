---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 4
api_specs:
- filename: agentcreditdata-com-agent-api-openapi.yml
  format: yaml
  label: Agent Credit Bureau Agent API
  slug: agentcreditdata-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentcreditdata-com/openapi/agentcreditdata-com-agent-api-openapi.yml
- filename: agentcreditdata-com-assess-api-openapi.yml
  format: yaml
  label: Agent Credit Bureau Assess API
  slug: agentcreditdata-com-assess-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentcreditdata-com/openapi/agentcreditdata-com-assess-api-openapi.yml
- filename: agentcreditdata-com-verify-api-openapi.yml
  format: yaml
  label: Agent Credit Bureau Verify API
  slug: agentcreditdata-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentcreditdata-com/openapi/agentcreditdata-com-verify-api-openapi.yml
consequence_counts:
  read: 4
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentcreditdata Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Agent Credit Bureau exposes 6 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agent Credit Bureau
provider_slug: agentcreditdata-com
slug: agentcreditdata-com-agentic-access
source_filename: agentcreditdata-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentcreditdata-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 4\n    acting: 2\n  by_consequence:\n    read: 4\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v0/agent/{id}\n  method: get\n  operationId: get_agent_identity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/agent/{id}/evidence\n  method: get\n  operationId: get_agent_evidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/agent/{id}/obligations\n\
  \  method: get\n  operationId: get_agent_obligations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/agent/{id}/credit-report\n  method: get\n  operationId: get_agent_credit_report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/assess\n  method: post\n  operationId: assess_agent_credit_exposure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/verify\n  method: post\n  operationId: verify_not_implemented\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agentcreditdata-com/agentic-access/agentcreditdata-com-agentic-access.yml
summary_line: 6 operations · 2 acting
tags:
- Company
- Finance
- Credit
- Artificial Intelligence
- Data
---

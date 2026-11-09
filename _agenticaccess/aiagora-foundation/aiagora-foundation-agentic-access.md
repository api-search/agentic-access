---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 4
api_specs:
- filename: aiagora-foundation-agents-api-openapi.yml
  format: yaml
  label: AIAgora Agents API
  slug: aiagora-foundation-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagora-foundation/openapi/aiagora-foundation-agents-api-openapi.yml
- filename: aiagora-foundation-health-api-openapi.yml
  format: yaml
  label: AIAgora Health API
  slug: aiagora-foundation-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagora-foundation/openapi/aiagora-foundation-health-api-openapi.yml
- filename: aiagora-foundation-hosts-api-openapi.yml
  format: yaml
  label: AIAgora Hosts API
  slug: aiagora-foundation-hosts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagora-foundation/openapi/aiagora-foundation-hosts-api-openapi.yml
- filename: aiagora-foundation-receipts-api-openapi.yml
  format: yaml
  label: AIAgora Receipts API
  slug: aiagora-foundation-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagora-foundation/openapi/aiagora-foundation-receipts-api-openapi.yml
- filename: aiagora-foundation-sandbox-api-openapi.yml
  format: yaml
  label: AIAgora Sandbox API
  slug: aiagora-foundation-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagora-foundation/openapi/aiagora-foundation-sandbox-api-openapi.yml
- filename: aiagora-foundation-stats-api-openapi.yml
  format: yaml
  label: AIAgora Stats API
  slug: aiagora-foundation-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiagora-foundation/openapi/aiagora-foundation-stats-api-openapi.yml
consequence_counts:
  physical: 1
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aiagora Foundation Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/hosts/messages
operation_count: 6
overview: 'AIAgora exposes 6 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AIAgora
provider_slug: aiagora-foundation
slug: aiagora-foundation-agentic-access
source_filename: aiagora-foundation-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/aiagora-foundation-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 4\n    acting: 2\n  by_consequence:\n    read: 4\n    write: 1\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/health\n  method: get\n  operationId: health_check_api_v1_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stats\n  method: get\n  operationId: get_stats_api_v1_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /api/v1/receipts/{receipt_id}\n  method: get\n  operationId: get_receipt_api_v1_receipts__receipt_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/dry-run\n  method: post\n  operationId: sandbox_dry_run_api_v1_sandbox_dry_run_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents\n  method: get\n  operationId: list_registered_agents_api_v1_agents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hosts/messages\n  method: post\n  operationId: send_host_message_api_v1_hosts_messages_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/aiagora-foundation/agentic-access/aiagora-foundation-agentic-access.yml
summary_line: 6 operations · 2 acting
tags:
- Artificial Intelligence
- Agents
- Collaboration
- Sandbox
- Open Platform
---

---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 7
api_specs:
- filename: agentrevenuenetwork-com-opportunities-api-openapi.yml
  format: yaml
  label: Agent Revenue Network Opportunities API
  slug: agentrevenuenetwork-com-opportunities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentrevenuenetwork-com/openapi/agentrevenuenetwork-com-opportunities-api-openapi.yml
- filename: agentrevenuenetwork-com-packages-api-openapi.yml
  format: yaml
  label: Agent Revenue Network Packages API
  slug: agentrevenuenetwork-com-packages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentrevenuenetwork-com/openapi/agentrevenuenetwork-com-packages-api-openapi.yml
- filename: agentrevenuenetwork-com-payment-guide-api-openapi.yml
  format: yaml
  label: Agent Revenue Network Payment Guide API
  slug: agentrevenuenetwork-com-payment-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentrevenuenetwork-com/openapi/agentrevenuenetwork-com-payment-guide-api-openapi.yml
- filename: agentrevenuenetwork-com-providers-api-openapi.yml
  format: yaml
  label: Agent Revenue Network Providers API
  slug: agentrevenuenetwork-com-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentrevenuenetwork-com/openapi/agentrevenuenetwork-com-providers-api-openapi.yml
- filename: agentrevenuenetwork-com-release-guard-api-openapi.yml
  format: yaml
  label: Agent Revenue Network Release Guard API
  slug: agentrevenuenetwork-com-release-guard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentrevenuenetwork-com/openapi/agentrevenuenetwork-com-release-guard-api-openapi.yml
- filename: agentrevenuenetwork-com-repeat-verification-api-openapi.yml
  format: yaml
  label: Agent Revenue Network Repeat Verification API
  slug: agentrevenuenetwork-com-repeat-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentrevenuenetwork-com/openapi/agentrevenuenetwork-com-repeat-verification-api-openapi.yml
- filename: agentrevenuenetwork-com-requests-api-openapi.yml
  format: yaml
  label: Agent Revenue Network Requests API
  slug: agentrevenuenetwork-com-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentrevenuenetwork-com/openapi/agentrevenuenetwork-com-requests-api-openapi.yml
- filename: agentrevenuenetwork-com-tools-api-openapi.yml
  format: yaml
  label: Agent Revenue Network Tools API
  slug: agentrevenuenetwork-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentrevenuenetwork-com/openapi/agentrevenuenetwork-com-tools-api-openapi.yml
consequence_counts:
  physical: 3
  read: 7
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentrevenuenetwork Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/release-guard/x402-access
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/release-guard/x402-starter
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/tools/json-normalize
operation_count: 25
overview: 'Agent Revenue Network exposes 25 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 15 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agent Revenue Network
provider_slug: agentrevenuenetwork-com
slug: agentrevenuenetwork-com-agentic-access
source_filename: agentrevenuenetwork-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentrevenuenetwork-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 7\n    acting: 18\n  by_consequence:\n    read: 7\n    physical: 3\n    write: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/tools\n  method: get\n  operationId: list_tools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/quality\n  method: get\n  operationId: get_tool_quality\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/packages/data-quality\n\
  \  method: get\n  operationId: get_data_quality_composition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/repeat-verification\n  method: get\n  operationId: get_repeat_verification_plan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/release-guard/config\n  method: get\n  operationId: get_release_guard_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/release-guard/x402-access\n  method: post\n  operationId: purchase_release_guard_x402_access\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/release-guard/x402-starter\n  method: post\n  operationId: purchase_release_guard_x402_starter\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/release-guard/verify\n  method: post\n  operationId: verify_release_subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/release-guard/receipts/{id}\n  method: get\n  operationId: verify_release_guard_receipt\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-guide\n  method: get\n  operationId: get_x402_payment_guide\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/requests\n  method: post\n  operationId: resolve_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/opportunities/score\n  method: post\n  operationId: score_opportunity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/providers/route\n  method: post\n  operationId: route_provider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/json-normalize\n  method: post\n  operationId: json_normalize\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/object-contract-check\n  method: post\n  operationId: object_contract_check\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/json-schema-check\n  method: post\n  operationId: json_schema_check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/json-diff\n  method: post\n  operationId: json_diff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/dataset-profile\n  method: post\n  operationId: dataset_profile\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/verify-execution\n  method: post\n  operationId: verify_execution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/release-evidence-diff\n  method: post\n  operationId: release_evidence_diff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/tools/verified-translation\n  method: post\n  operationId: verified_translation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/result-dedupe\n  method: post\n  operationId: result_dedupe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/schema-infer\n  method: post\n  operationId: schema_infer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/tabular-diff\n  method: post\n  operationId: tabular_diff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/tabular-validate\n  method: post\n  operationId: tabular_validate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agentrevenuenetwork-com/agentic-access/agentrevenuenetwork-com-agentic-access.yml
summary_line: 25 operations · 18 acting
tags:
- Artificial Intelligence
- Finance
- MCP
- Tools
---

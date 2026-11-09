---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 8
api_specs:
- filename: synlake-ai-auth-api-openapi.yml
  format: yaml
  label: synlake-ai Auth API
  slug: synlake-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synlake-ai/openapi/synlake-ai-auth-api-openapi.yml
- filename: synlake-ai-billing-api-openapi.yml
  format: yaml
  label: synlake-ai Billing API
  slug: synlake-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synlake-ai/openapi/synlake-ai-billing-api-openapi.yml
- filename: synlake-ai-catalog-api-openapi.yml
  format: yaml
  label: synlake-ai Catalog API
  slug: synlake-ai-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synlake-ai/openapi/synlake-ai-catalog-api-openapi.yml
- filename: synlake-ai-execution-api-openapi.yml
  format: yaml
  label: synlake-ai Execution API
  slug: synlake-ai-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synlake-ai/openapi/synlake-ai-execution-api-openapi.yml
- filename: synlake-ai-infrastructure-api-openapi.yml
  format: yaml
  label: synlake-ai Infrastructure API
  slug: synlake-ai-infrastructure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synlake-ai/openapi/synlake-ai-infrastructure-api-openapi.yml
- filename: synlake-ai-system-api-openapi.yml
  format: yaml
  label: synlake-ai System API
  slug: synlake-ai-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synlake-ai/openapi/synlake-ai-system-api-openapi.yml
consequence_counts:
  read: 8
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Synlake Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'synlake-ai exposes 16 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: synlake-ai
provider_slug: synlake-ai
slug: synlake-ai-agentic-access
source_filename: synlake-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/api-synlake-openapi.json, openapi/synlake-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 8\n    connected: 8\n  by_consequence:\n    write: 8\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /register\n  method: post\n  operationId: registerAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /infrastructure/query\n  method: post\n  operationId: queryInfrastructure\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infrastructure/estimate\n  method: post\n  operationId: estimateCost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execution/validate\n  method: post\n  operationId: validateExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers\n  method: get\n  operationId: listProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/activate\n  method: post\n  operationId: activateBilling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /register\n  method: post\n  operationId: registerAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /infrastructure/query\n  method: post\n  operationId: queryInfrastructure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infrastructure/estimate\n  method: post\n  operationId: estimateCost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execution/validate\n  method: post\n  operationId: validateExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers\n  method: get\n  operationId: listProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/activate\n  method: post\n  operationId: activateBilling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/synlake-ai/agentic-access/synlake-ai-agentic-access.yml
summary_line: 16 operations · 8 acting
tags:
- Company
- Data Infrastructure
- AI Agents
- Cloud
- Terraform
---

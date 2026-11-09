---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 6
api_specs:
- filename: modelcostcomparison-com-ai-benchmarks-snapshot-json-api-openapi.yml
  format: yaml
  label: Model Cost Comparison Ai Benchmarks Snapshot.json API
  slug: modelcostcomparison-com-ai-benchmarks-snapshot-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelcostcomparison-com/openapi/modelcostcomparison-com-ai-benchmarks-snapshot-json-api-openapi.yml
- filename: modelcostcomparison-com-ai-provider-pricing-validated-json-api-openapi.yml
  format: yaml
  label: Model Cost Comparison Ai Provider Pricing Validated.json API
  slug: modelcostcomparison-com-ai-provider-pricing-validated-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelcostcomparison-com/openapi/modelcostcomparison-com-ai-provider-pricing-validated-json-api-openapi.yml
- filename: modelcostcomparison-com-cron-api-openapi.yml
  format: yaml
  label: Model Cost Comparison Cron API
  slug: modelcostcomparison-com-cron-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelcostcomparison-com/openapi/modelcostcomparison-com-cron-api-openapi.yml
- filename: modelcostcomparison-com-llms-txt-api-openapi.yml
  format: yaml
  label: Model Cost Comparison Llms.txt API
  slug: modelcostcomparison-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelcostcomparison-com/openapi/modelcostcomparison-com-llms-txt-api-openapi.yml
- filename: modelcostcomparison-com-mcc-model-advisor-api-openapi.yml
  format: yaml
  label: Model Cost Comparison Mcc Model Advisor API
  slug: modelcostcomparison-com-mcc-model-advisor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelcostcomparison-com/openapi/modelcostcomparison-com-mcc-model-advisor-api-openapi.yml
- filename: modelcostcomparison-com-model-cost-comparison-api-api-openapi.yml
  format: yaml
  label: Model Cost Comparison Model Cost Comparison API
  slug: modelcostcomparison-com-model-cost-comparison-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelcostcomparison-com/openapi/modelcostcomparison-com-model-cost-comparison-api-api-openapi.yml
- filename: modelcostcomparison-com-models-api-openapi.yml
  format: yaml
  label: Model Cost Comparison Models API
  slug: modelcostcomparison-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelcostcomparison-com/openapi/modelcostcomparison-com-models-api-openapi.yml
consequence_counts:
  read: 6
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Modelcostcomparison Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Model Cost Comparison exposes 8 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Model Cost Comparison
provider_slug: modelcostcomparison-com
slug: modelcostcomparison-com-agentic-access
source_filename: modelcostcomparison-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/modelcostcomparison-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 6\n    acting: 2\n  by_consequence:\n    read: 6\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1\n  method: get\n  operationId: apiV1Index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/models/advisor\n  method: post\n  operationId: mccModelAdvisorV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/models/advisor\n  method: get\n  operationId: mccModelAdvisorV1WrongMethod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cron/trigger-ai-pricing-refresh\n  method: get\n  operationId: triggerPricingRefreshV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcc-model-advisor\n  method: post\n  operationId: mccModelAdvisorLegacy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /llms.txt\n  method: get\n  operationId: llmsTxt\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai-provider-pricing-validated.json\n  method: get\n  operationId: pricingDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai-benchmarks-snapshot.json\n  method: get\n  operationId: benchmarksSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/modelcostcomparison-com/agentic-access/modelcostcomparison-com-agentic-access.yml
summary_line: 8 operations · 2 acting
tags:
- Artificial Intelligence
- Cost Comparison
- LLM
- Pricing
- Calculator
---

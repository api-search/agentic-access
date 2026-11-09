---
acting_count: 10
action_class_counts:
  acting: 10
api_specs:
- filename: ontoramp-com-commerce-api-openapi.yml
  format: yaml
  label: ontoramp-com Commerce API
  slug: ontoramp-com-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ontoramp-com/openapi/ontoramp-com-commerce-api-openapi.yml
- filename: ontoramp-com-decision-intelligence-api-openapi.yml
  format: yaml
  label: ontoramp-com Decision Intelligence API
  slug: ontoramp-com-decision-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ontoramp-com/openapi/ontoramp-com-decision-intelligence-api-openapi.yml
- filename: ontoramp-com-governance-evaluator-api-openapi.yml
  format: yaml
  label: ontoramp-com Governance Evaluator API
  slug: ontoramp-com-governance-evaluator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ontoramp-com/openapi/ontoramp-com-governance-evaluator-api-openapi.yml
- filename: ontoramp-com-knowledge-graph-api-openapi.yml
  format: yaml
  label: ontoramp-com Knowledge Graph API
  slug: ontoramp-com-knowledge-graph-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ontoramp-com/openapi/ontoramp-com-knowledge-graph-api-openapi.yml
- filename: ontoramp-com-projection-engine-api-openapi.yml
  format: yaml
  label: ontoramp-com Projection Engine API
  slug: ontoramp-com-projection-engine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ontoramp-com/openapi/ontoramp-com-projection-engine-api-openapi.yml
consequence_counts:
  physical: 2
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ontoramp Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/checkout
operation_count: 10
overview: 'ontoramp-com exposes 10 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 write and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ontoramp-com
provider_slug: ontoramp-com
slug: ontoramp-com-agentic-access
source_filename: ontoramp-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/ontoramp-com-openapi.yaml, openapi/ontoramp-com.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 10\n  by_consequence:\n    write: 8\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /knowledge-graph/mcp\n  method: post\n  operationId: knowledgeGraph\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /governance-evaluator/mcp\n  method: post\n  operationId: governanceEvaluator\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projection-engine/mcp\n  method: post\n  operationId: projectionEngine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /decision-intelligence/mcp\n  method: post\n  operationId: decisionIntelligence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/checkout\n\
  \  method: post\n  operationId: createCheckoutLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /knowledge-graph/mcp\n  method: post\n  operationId: knowledgeGraph\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /governance-evaluator/mcp\n  method: post\n  operationId: governanceEvaluator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projection-engine/mcp\n  method: post\n  operationId: projectionEngine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /decision-intelligence/mcp\n  method: post\n  operationId: decisionIntelligence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/checkout\n  method: post\n  operationId: createCheckoutLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/ontoramp-com/agentic-access/ontoramp-com-agentic-access.yml
summary_line: 10 operations · 10 acting
tags:
- Company
- AI Governance
- AI Agents
- Compliance
- Certification
---

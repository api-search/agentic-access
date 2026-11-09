---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: canonicai-com-answers-api-openapi.yml
  format: yaml
  label: CanonicAI Answers API
  slug: canonicai-com-answers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canonicai-com/openapi/canonicai-com-answers-api-openapi.yml
- filename: canonicai-com-canons-api-openapi.yml
  format: yaml
  label: CanonicAI Canons API
  slug: canonicai-com-canons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canonicai-com/openapi/canonicai-com-canons-api-openapi.yml
- filename: canonicai-com-llms-txt-api-openapi.yml
  format: yaml
  label: CanonicAI Llms.txt API
  slug: canonicai-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canonicai-com/openapi/canonicai-com-llms-txt-api-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Canonicai Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'CanonicAI exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CanonicAI
provider_slug: canonicai-com
slug: canonicai-com-agentic-access
source_filename: canonicai-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/canonicai-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /answers/index.json\n  method: get\n  operationId: listAnswers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /answers/{slug}.json\n  method: get\n  operationId: getAnswerStatic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/answers\n  method: get\n  operationId: listAnswersApi\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/answers/search\n  method: get\n  operationId: searchAnswersApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/answers/{slug}\n  method: get\n  operationId: getAnswerApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/canons\n  method: get\n  operationId: listCanonsApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/canons/search\n  method: get\n  operationId: searchConstructsApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/canons/{slug}\n  method: get\n  operationId: getCanonApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: llmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/canonicai-com/agentic-access/canonicai-com-agentic-access.yml
summary_line: 9 operations
tags:
- Company
- Artificial Intelligence
- Data Extraction
- Tagging
- CanonicalDatasets
- Automation
---

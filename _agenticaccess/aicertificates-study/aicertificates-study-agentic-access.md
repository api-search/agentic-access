---
acting_count: 0
action_class_counts:
  connected: 3
api_specs:
- filename: aicertificates-study-content-api-openapi.yml
  format: yaml
  label: AI Certificates Content API
  slug: aicertificates-study-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicertificates-study/openapi/aicertificates-study-content-api-openapi.yml
- filename: aicertificates-study-readiness-api-openapi.yml
  format: yaml
  label: AI Certificates Readiness API
  slug: aicertificates-study-readiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicertificates-study/openapi/aicertificates-study-readiness-api-openapi.yml
consequence_counts:
  read: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aicertificates Study Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'AI Certificates exposes 3 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AI Certificates
provider_slug: aicertificates-study
slug: aicertificates-study-agentic-access
source_filename: aicertificates-study-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/aicertificates-study-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    connected: 3\n  by_consequence:\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/readiness-stats\n  method: get\n  operationId: getReadinessStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/readiness-token\n  method: get\n  operationId: mintReadinessToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /md/{slug}\n  method: get\n  operationId:\
  \ getGuideMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/aicertificates-study/agentic-access/aicertificates-study-agentic-access.yml
summary_line: 3 operations
tags:
- Education
- Artificial Intelligence
- Certification
- Practice Exams
- Anthropic
---

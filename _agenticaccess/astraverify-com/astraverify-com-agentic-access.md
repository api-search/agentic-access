---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 4
api_specs:
- filename: astraverify-com-discoverability-api-openapi.yml
  format: yaml
  label: AstraVerify Discoverability API
  slug: astraverify-com-discoverability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraverify-com/openapi/astraverify-com-discoverability-api-openapi.yml
- filename: astraverify-com-email-api-openapi.yml
  format: yaml
  label: AstraVerify Email API
  slug: astraverify-com-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraverify-com/openapi/astraverify-com-email-api-openapi.yml
- filename: astraverify-com-fetch-as-api-openapi.yml
  format: yaml
  label: AstraVerify Fetch As API
  slug: astraverify-com-fetch-as-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraverify-com/openapi/astraverify-com-fetch-as-api-openapi.yml
- filename: astraverify-com-report-api-openapi.yml
  format: yaml
  label: AstraVerify Report API
  slug: astraverify-com-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraverify-com/openapi/astraverify-com-report-api-openapi.yml
- filename: astraverify-com-verify-api-openapi.yml
  format: yaml
  label: AstraVerify Verify API
  slug: astraverify-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraverify-com/openapi/astraverify-com-verify-api-openapi.yml
consequence_counts:
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Astraverify Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'AstraVerify exposes 5 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AstraVerify
provider_slug: astraverify-com
slug: astraverify-com-agentic-access
source_filename: astraverify-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/astraverify-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 4\n    acting: 1\n  by_consequence:\n    read: 4\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/discoverability\n  method: get\n  operationId: checkDiscoverability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/email\n  method: get\n  operationId: checkEmailSecurity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fetch-as\n\
  \  method: get\n  operationId: fetchAsCrawler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/report\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/verify\n  method: post\n  operationId: verifyFix\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/astraverify-com/agentic-access/astraverify-com-agentic-access.yml
summary_line: 5 operations · 1 acting
tags:
- Security
- Email
- Artificial Intelligence
- Discoverability
- Domain
---

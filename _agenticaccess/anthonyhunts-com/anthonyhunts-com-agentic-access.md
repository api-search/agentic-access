---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 5
api_specs:
- filename: anthonyhunts-com-batch-api-openapi.yml
  format: yaml
  label: anthonyhunts-com Batch API
  slug: anthonyhunts-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthonyhunts-com/openapi/anthonyhunts-com-batch-api-openapi.yml
- filename: anthonyhunts-com-contact-api-openapi.yml
  format: yaml
  label: anthonyhunts-com Contact API
  slug: anthonyhunts-com-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthonyhunts-com/openapi/anthonyhunts-com-contact-api-openapi.yml
- filename: anthonyhunts-com-content-api-openapi.yml
  format: yaml
  label: anthonyhunts-com Content API
  slug: anthonyhunts-com-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthonyhunts-com/openapi/anthonyhunts-com-content-api-openapi.yml
- filename: anthonyhunts-com-pricing-api-openapi.yml
  format: yaml
  label: anthonyhunts-com Pricing API
  slug: anthonyhunts-com-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthonyhunts-com/openapi/anthonyhunts-com-pricing-api-openapi.yml
- filename: anthonyhunts-com-search-api-openapi.yml
  format: yaml
  label: anthonyhunts-com Search API
  slug: anthonyhunts-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthonyhunts-com/openapi/anthonyhunts-com-search-api-openapi.yml
- filename: anthonyhunts-com-services-api-openapi.yml
  format: yaml
  label: anthonyhunts-com Services API
  slug: anthonyhunts-com-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthonyhunts-com/openapi/anthonyhunts-com-services-api-openapi.yml
consequence_counts:
  read: 5
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Anthonyhunts Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'anthonyhunts-com exposes 7 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: anthonyhunts-com
provider_slug: anthonyhunts-com
slug: anthonyhunts-com-agentic-access
source_filename: anthonyhunts-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/anthonyhunts-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 5\n    acting: 2\n  by_consequence:\n    read: 5\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/pricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/capabilities\n  method: get\n  operationId: listCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/contact\n  method:\
  \ get\n  operationId: getContactOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/posts\n  method: get\n  operationId: listPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/batch\n  method: post\n  operationId: batchGet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ask\n  method: post\n  operationId: askSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /{path}\n  method: get\n  operationId: getPageMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/anthonyhunts-com/agentic-access/anthonyhunts-com-agentic-access.yml
summary_line: 7 operations · 2 acting
tags:
- Company
- Marketing
- Artificial Intelligence
- Automation
- Latin America
- US
---

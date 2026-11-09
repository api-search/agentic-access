---
acting_count: 1
action_class_counts:
  acting: 1
api_specs:
- filename: html2img-com-account-api-openapi.yml
  format: yaml
  label: html2img-com Account API
  slug: html2img-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/html2img-com/openapi/html2img-com-account-api-openapi.yml
- filename: html2img-com-html-rendering-api-openapi.yml
  format: yaml
  label: html2img-com HTML rendering API
  slug: html2img-com-html-rendering-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/html2img-com/openapi/html2img-com-html-rendering-api-openapi.yml
- filename: html2img-com-screenshots-api-openapi.yml
  format: yaml
  label: html2img-com Screenshots API
  slug: html2img-com-screenshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/html2img-com/openapi/html2img-com-screenshots-api-openapi.yml
- filename: html2img-com-templates-api-openapi.yml
  format: yaml
  label: html2img-com Templates API
  slug: html2img-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/html2img-com/openapi/html2img-com-templates-api-openapi.yml
consequence_counts:
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Html2Img Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 1
overview: 'html2img-com exposes 1 API operation that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: html2img-com
provider_slug: html2img-com
slug: html2img-com-agentic-access
source_filename: html2img-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/html2img-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1\n  by_action_class:\n    acting: 1\n  by_consequence:\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /html\n  method: post\n  operationId: renderHtml\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/html2img-com/agentic-access/html2img-com-agentic-access.yml
summary_line: 1 operation · 1 acting
tags:
- Company
- Screenshots
- PDF
- Rendering
- Headless Chrome
---

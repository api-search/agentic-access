---
acting_count: 4
action_class_counts:
  acting: 4
api_specs:
- filename: apiaddicts-configuration-api-openapi.yml
  format: yaml
  label: apIAddicts Configuration API
  slug: apiaddicts-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiaddicts/refs/heads/main/openapi/apiaddicts-configuration-api-openapi.yml
- filename: apiaddicts-generator-api-openapi.yml
  format: yaml
  label: apIAddicts Generator API
  slug: apiaddicts-generator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiaddicts/refs/heads/main/openapi/apiaddicts-generator-api-openapi.yml
- filename: apiaddicts-soapui-api-openapi.yml
  format: yaml
  label: apIAddicts Soap UI API
  slug: apiaddicts-soapui-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiaddicts/refs/heads/main/openapi/apiaddicts-soapui-api-openapi.yml
consequence_counts:
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Apiaddicts Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'apIAddicts exposes 4 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: apIAddicts
provider_slug: apiaddicts
slug: apiaddicts-agentic-access
source_filename: apiaddicts-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: generated\nsource: openapi/apiaddicts-apigen-openapi.yml, openapi/apiaddicts-openapi2soapui-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 4\n  by_consequence:\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /configuration/file\n  method: post\n  operationId: configurationFromFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generator/config\n  method: post\n  operationId: generateFromConfig\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generator/file\n  method: post\n  operationId: generateFromFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /soap-ui-projects\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiaddicts/refs/heads/main/agentic-access/apiaddicts-agentic-access.yml
summary_line: 4 operations · 4 acting
tags:
- Company
- Non-Profit
- Community
- API Training
- Certification
- Events
- Open Source
- API Governance
- Spectral
- MCP
---

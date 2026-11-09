---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 5
api_specs:
- filename: onlinecompiler-io-account-api-openapi.yml
  format: yaml
  label: onlinecompiler-io Account API
  slug: onlinecompiler-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onlinecompiler-io/openapi/onlinecompiler-io-account-api-openapi.yml
- filename: onlinecompiler-io-judge-api-openapi.yml
  format: yaml
  label: onlinecompiler-io Judge API
  slug: onlinecompiler-io-judge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onlinecompiler-io/openapi/onlinecompiler-io-judge-api-openapi.yml
- filename: onlinecompiler-io-reference-api-openapi.yml
  format: yaml
  label: onlinecompiler-io Reference API
  slug: onlinecompiler-io-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onlinecompiler-io/openapi/onlinecompiler-io-reference-api-openapi.yml
- filename: onlinecompiler-io-run-api-openapi.yml
  format: yaml
  label: onlinecompiler-io Run API
  slug: onlinecompiler-io-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onlinecompiler-io/openapi/onlinecompiler-io-run-api-openapi.yml
consequence_counts:
  read: 5
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Onlinecompiler Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'onlinecompiler-io exposes 8 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: onlinecompiler-io
provider_slug: onlinecompiler-io
slug: onlinecompiler-io-agentic-access
source_filename: onlinecompiler-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/api.onlinecompiler.io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 3\n    connected: 5\n  by_consequence:\n    write: 3\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/run-code-sync/\n  method: post\n  operationId: runCodeSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/run-code/\n  method: post\n  operationId: runCodeAsync\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/run-tests/\n  method: post\n  operationId: runTests\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/compilers/\n  method: get\n  operationId: listCompilers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/limits/\n  method: get\n  operationId: getLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/usage/\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health/\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/files/{file_id}/\n  method: get\n  operationId: downloadFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/onlinecompiler-io/agentic-access/onlinecompiler-io-agentic-access.yml
summary_line: 8 operations · 3 acting
tags:
- Company
- Code Execution
- Developer Tools
- Education
- Artificial Intelligence
---

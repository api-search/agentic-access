---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 3
api_specs:
- filename: letagentsin-com-c-api-openapi.yml
  format: yaml
  label: letagentsin-com C API
  slug: letagentsin-com-c-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letagentsin-com/openapi/letagentsin-com-c-api-openapi.yml
- filename: letagentsin-com-corpus-csv-api-openapi.yml
  format: yaml
  label: letagentsin-com Corpus.csv API
  slug: letagentsin-com-corpus-csv-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letagentsin-com/openapi/letagentsin-com-corpus-csv-api-openapi.yml
- filename: letagentsin-com-corpus-json-api-openapi.yml
  format: yaml
  label: letagentsin-com Corpus.json API
  slug: letagentsin-com-corpus-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letagentsin-com/openapi/letagentsin-com-corpus-json-api-openapi.yml
- filename: letagentsin-com-mcp-api-openapi.yml
  format: yaml
  label: letagentsin-com MCP API
  slug: letagentsin-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letagentsin-com/openapi/letagentsin-com-mcp-api-openapi.yml
- filename: letagentsin-com-scan-api-openapi.yml
  format: yaml
  label: letagentsin-com Scan API
  slug: letagentsin-com-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letagentsin-com/openapi/letagentsin-com-scan-api-openapi.yml
- filename: letagentsin-com-visibility-api-openapi.yml
  format: yaml
  label: letagentsin-com Visibility API
  slug: letagentsin-com-visibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letagentsin-com/openapi/letagentsin-com-visibility-api-openapi.yml
- filename: letagentsin-com-watch-api-openapi.yml
  format: yaml
  label: letagentsin-com Watch API
  slug: letagentsin-com-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letagentsin-com/openapi/letagentsin-com-watch-api-openapi.yml
consequence_counts:
  read: 3
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Letagentsin Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'letagentsin-com exposes 9 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: letagentsin-com
provider_slug: letagentsin-com
slug: letagentsin-com-agentic-access
source_filename: letagentsin-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/letagentsin-com-openapi.json, openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 6\n    connected: 3\n  by_consequence:\n    write: 6\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/scan\n  method: post\n  operationId: scanDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/scan\n  method: post\n  operationId: scanDomain\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/scan/stream\n  method: post\n  operationId: scanDomainStreaming\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/watch\n  method: post\n  operationId: watchDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /corpus.json\n  method: get\n  operationId: getCorpus\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /corpus.csv\n  method: get\n  operationId: getCorpusCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /c/{category}/corpus.json\n  method: get\n  operationId: getCategoryCorpus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/visibility\n  method: post\n  operationId: auditAiVisibility\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: mcpJsonRpc\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/letagentsin-com/agentic-access/letagentsin-com-agentic-access.yml
summary_line: 9 operations · 6 acting
tags:
- Artificial Intelligence
- Agent Audits
- Developer Tools
- API Testing
- Integration
---

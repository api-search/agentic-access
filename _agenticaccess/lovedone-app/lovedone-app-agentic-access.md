---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 15
api_specs:
- filename: lovedone-app-content-api-openapi.yml
  format: yaml
  label: lovedone-app Content API
  slug: lovedone-app-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lovedone-app/openapi/lovedone-app-content-api-openapi.yml
- filename: lovedone-app-discovery-api-openapi.yml
  format: yaml
  label: lovedone-app Discovery API
  slug: lovedone-app-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lovedone-app/openapi/lovedone-app-discovery-api-openapi.yml
- filename: lovedone-app-mcp-api-openapi.yml
  format: yaml
  label: lovedone-app MCP API
  slug: lovedone-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lovedone-app/openapi/lovedone-app-mcp-api-openapi.yml
consequence_counts:
  read: 15
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lovedone App Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'lovedone-app exposes 16 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: lovedone-app
provider_slug: lovedone-app
slug: lovedone-app-agentic-access
source_filename: lovedone-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/lovedone-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 15\n    acting: 1\n  by_consequence:\n    read: 15\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /openapi.json\n  method: get\n  operationId: getOpenApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/openapi.json\n  method: get\n  operationId: getOpenApiAlias\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n\
  \  operationId: getLlmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sitemap.xml\n  method: get\n  operationId: getSitemap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /robots.txt\n  method: get\n  operationId: getRobots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp/server.json\n  method: get\n  operationId: getMcpManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getHome\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /about\n  method: get\n  operationId: getAbout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /our-brands\n  method: get\n  operationId: getOurBrands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getting-started\n  method: get\n  operationId: getGettingStarted\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /for-providers\n  method: get\n  operationId: getForProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blog\n  method: get\n  operationId: getBlog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /privacy\n  method: get\n  operationId: getPrivacy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /terms\n  method: get\n  operationId: getTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/v1\n  method: get\n  operationId: getMcpProbe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/v1\n  method: post\n  operationId: postMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - care_circle:read\n    - profile:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/lovedone-app/agentic-access/lovedone-app-agentic-access.yml
summary_line: 16 operations · 1 acting
tags:
- Family Care
- Inbox
- Healthcare
- Communications
- Privacy
---

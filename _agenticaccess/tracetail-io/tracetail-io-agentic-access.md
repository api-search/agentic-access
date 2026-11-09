---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 5
api_specs:
- filename: tracetail-io-identification-api-openapi.yml
  format: yaml
  label: tracetail-io Identification API
  slug: tracetail-io-identification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tracetail-io/openapi/tracetail-io-identification-api-openapi.yml
- filename: tracetail-io-server-api-api-openapi.yml
  format: yaml
  label: tracetail-io Server API
  slug: tracetail-io-server-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tracetail-io/openapi/tracetail-io-server-api-api-openapi.yml
- filename: tracetail-io-service-api-openapi.yml
  format: yaml
  label: tracetail-io Service API
  slug: tracetail-io-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tracetail-io/openapi/tracetail-io-service-api-openapi.yml
- filename: tracetail-io-setup-links-api-openapi.yml
  format: yaml
  label: tracetail-io Setup links API
  slug: tracetail-io-setup-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tracetail-io/openapi/tracetail-io-setup-links-api-openapi.yml
consequence_counts:
  read: 5
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tracetail Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'tracetail-io exposes 8 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: tracetail-io
provider_slug: tracetail-io
slug: tracetail-io-agentic-access
source_filename: tracetail-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/tracetail-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 3\n    connected: 5\n  by_consequence:\n    write: 3\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/id\n  method: post\n  operationId: identify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/id/detail\n  method: post\n  operationId: identifyDetailed\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/identifications/{requestId}\n  method: get\n  operationId: getIdentification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/visitors/{visitorId}\n  method: get\n  operationId: getVisitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/setup-links\n  method: post\n  operationId: createSetupLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /api/v1/setup-links/{setupLinkId}\n  method: get\n  operationId: checkSetupLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/proxy/status\n  method: get\n  operationId: getProxyStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/tracetail-io/agentic-access/tracetail-io-agentic-access.yml
summary_line: 8 operations · 3 acting
tags:
- Browser Fingerprinting
- Privacy
- Analytics
- Device Identification
---

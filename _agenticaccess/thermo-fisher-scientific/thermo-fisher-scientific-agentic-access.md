---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 9
api_specs:
- filename: thermo-fisher-scientific-authentication-api-openapi.yml
  format: yaml
  label: Thermo Fisher Scientific Authentication API
  slug: thermo-fisher-scientific-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-scientific-authentication-api-openapi.yml
- filename: thermo-fisher-scientific-entities-api-openapi.yml
  format: yaml
  label: Thermo Fisher Scientific Entities API
  slug: thermo-fisher-scientific-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-scientific-entities-api-openapi.yml
- filename: thermo-fisher-scientific-export-api-openapi.yml
  format: yaml
  label: Thermo Fisher Scientific Export API
  slug: thermo-fisher-scientific-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-scientific-export-api-openapi.yml
- filename: thermo-fisher-scientific-instrument-api-openapi.yml
  format: yaml
  label: Thermo Fisher Scientific Instrument API
  slug: thermo-fisher-scientific-instrument-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-scientific-instrument-api-openapi.yml
- filename: thermo-fisher-scientific-measurements-api-openapi.yml
  format: yaml
  label: Thermo Fisher Scientific Measurements API
  slug: thermo-fisher-scientific-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-scientific-measurements-api-openapi.yml
- filename: thermo-fisher-scientific-methods-api-openapi.yml
  format: yaml
  label: Thermo Fisher Scientific Methods API
  slug: thermo-fisher-scientific-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-scientific-methods-api-openapi.yml
- filename: thermo-fisher-scientific-results-api-openapi.yml
  format: yaml
  label: Thermo Fisher Scientific Results API
  slug: thermo-fisher-scientific-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-scientific-results-api-openapi.yml
- filename: thermo-fisher-scientific-samples-api-openapi.yml
  format: yaml
  label: Thermo Fisher Scientific Samples API
  slug: thermo-fisher-scientific-samples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-scientific-samples-api-openapi.yml
- filename: thermo-fisher-scientific-workflows-api-openapi.yml
  format: yaml
  label: Thermo Fisher Scientific Workflows API
  slug: thermo-fisher-scientific-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-scientific-workflows-api-openapi.yml
consequence_counts:
  read: 9
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Thermo Fisher Scientific Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Thermo Fisher Scientific exposes 15 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Thermo Fisher Scientific
provider_slug: thermo-fisher-scientific
slug: thermo-fisher-scientific-agentic-access
source_filename: thermo-fisher-scientific-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/thermo-fisher-nanodrop-openapi.yml, openapi/thermo-fisher-samplemanager-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 9\n    acting: 6\n  by_consequence:\n    read: 9\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/status\n  method: get\n  operationId: getInstrumentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/measure\n  method: post\n  operationId: performMeasurement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/measurements\n  method: get\n  operationId: getMeasurements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/measurements/{measurementId}\n  method: get\n  operationId: getMeasurementById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/methods\n  method: get\n  operationId: getMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/export\n  method: post\n  operationId: exportMeasurements\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mobile/login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mobile/logout\n  method: post\n  operationId: logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mobile/browses/{entity}\n  method: get\n  operationId: browseEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mobile/browses/{entity}/{id}\n  method: get\n  operationId: getEntityById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mobile/samples\n  method: get\n  operationId: getSamples\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mobile/samples/{sampleId}\n  method: get\n  operationId: getSampleById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mobile/samples/{sampleId}/results\n  method: get\n  operationId: getSampleResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mobile/results\n\
  \  method: post\n  operationId: submitResults\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mobile/workflows/{workflowName}/trigger\n  method: post\n  operationId: triggerWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/agentic-access/thermo-fisher-scientific-agentic-access.yml
summary_line: 15 operations · 6 acting
tags:
- Life Sciences
- Laboratory
- Scientific Instruments
- LIMS
- Diagnostics
- Biosciences
- Fortune 500
---

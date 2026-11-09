---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 12
api_specs:
- filename: cfsoft-us-batch-api-openapi.yml
  format: yaml
  label: cfsoft-us Batch API
  slug: cfsoft-us-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cfsoft-us/openapi/cfsoft-us-batch-api-openapi.yml
- filename: cfsoft-us-check-api-openapi.yml
  format: yaml
  label: cfsoft-us Check API
  slug: cfsoft-us-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cfsoft-us/openapi/cfsoft-us-check-api-openapi.yml
- filename: cfsoft-us-health-api-openapi.yml
  format: yaml
  label: cfsoft-us Health API
  slug: cfsoft-us-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cfsoft-us/openapi/cfsoft-us-health-api-openapi.yml
- filename: cfsoft-us-report-api-openapi.yml
  format: yaml
  label: cfsoft-us Report API
  slug: cfsoft-us-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cfsoft-us/openapi/cfsoft-us-report-api-openapi.yml
- filename: cfsoft-us-well-known-api-openapi.yml
  format: yaml
  label: cfsoft-us .well Known API
  slug: cfsoft-us-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cfsoft-us/openapi/cfsoft-us-well-known-api-openapi.yml
consequence_counts:
  read: 12
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cfsoft Us Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'cfsoft-us exposes 13 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: cfsoft-us
provider_slug: cfsoft-us
slug: cfsoft-us-agentic-access
source_filename: cfsoft-us-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/enforcement-openapi.json, openapi/exclusions-openapi.json, openapi/packages-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 12\n    acting: 1\n  by_consequence:\n    read: 12\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/check\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/report\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/x402\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/check\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/report\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/health\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/x402\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/check\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/report\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/x402\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cfsoft-us/agentic-access/cfsoft-us-agentic-access.yml
summary_line: 13 operations · 1 acting
tags:
- Company
- Artificial Intelligence
- Finance
- Legal
---

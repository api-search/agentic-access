---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 7
api_specs:
- filename: imejis-io-analytics-api-openapi.yml
  format: yaml
  label: imejis-io Analytics API
  slug: imejis-io-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imejis-io/openapi/imejis-io-analytics-api-openapi.yml
- filename: imejis-io-designs-api-openapi.yml
  format: yaml
  label: imejis-io Designs API
  slug: imejis-io-designs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imejis-io/openapi/imejis-io-designs-api-openapi.yml
- filename: imejis-io-keys-api-openapi.yml
  format: yaml
  label: imejis-io Keys API
  slug: imejis-io-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imejis-io/openapi/imejis-io-keys-api-openapi.yml
- filename: imejis-io-render-api-openapi.yml
  format: yaml
  label: imejis-io Render API
  slug: imejis-io-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imejis-io/openapi/imejis-io-render-api-openapi.yml
consequence_counts:
  read: 7
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Imejis Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'imejis-io exposes 13 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: imejis-io
provider_slug: imejis-io
slug: imejis-io-agentic-access
source_filename: imejis-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/imejis-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 7\n    acting: 6\n  by_consequence:\n    read: 7\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /{design_id}\n  method: get\n  operationId: renderDesignGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{design_id}\n  method: post\n  operationId: renderDesignPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulk\n  method: post\n  operationId: bulkExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /designs/v2\n  method: get\n  operationId: listDesigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /designs/v2/{id}\n  method: get\n  operationId: getDesign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /designs/v2/{id}/config\n  method: get\n  operationId: getDesignRenderConfig\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /designs/v2/{id}/export\n  method: post\n  operationId: exportDesign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /designs/v2/{id}/export/driver-upload\n  method: post\n  operationId: exportDesignHosted\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /designs/v2/{id}/export/signed-url\n  method: post\n  operationId: exportDesignSigned\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /designs/v2/{id}/export/jobs\n  method: post\n  operationId: exportDesignAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/exports/{exportId}\n  method: get\n  operationId: getExportJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/api\n  method: get\n  operationId: getApiUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/api-keys\n\
  \  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/imejis-io/agentic-access/imejis-io-agentic-access.yml
summary_line: 13 operations · 6 acting
tags:
- Company
---

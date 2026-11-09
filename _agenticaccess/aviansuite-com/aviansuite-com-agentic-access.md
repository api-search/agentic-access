---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 8
api_specs:
- filename: aviansuite-com-admin-api-openapi.yml
  format: yaml
  label: AvianSuite Admin API
  slug: aviansuite-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviansuite-com/openapi/aviansuite-com-admin-api-openapi.yml
- filename: aviansuite-com-events-api-openapi.yml
  format: yaml
  label: AvianSuite Events API
  slug: aviansuite-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviansuite-com/openapi/aviansuite-com-events-api-openapi.yml
- filename: aviansuite-com-health-api-openapi.yml
  format: yaml
  label: AvianSuite Health API
  slug: aviansuite-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviansuite-com/openapi/aviansuite-com-health-api-openapi.yml
- filename: aviansuite-com-refs-api-openapi.yml
  format: yaml
  label: AvianSuite Refs API
  slug: aviansuite-com-refs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviansuite-com/openapi/aviansuite-com-refs-api-openapi.yml
- filename: aviansuite-com-root-api-openapi.yml
  format: yaml
  label: AvianSuite Root API
  slug: aviansuite-com-root-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviansuite-com/openapi/aviansuite-com-root-api-openapi.yml
consequence_counts:
  read: 8
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aviansuite Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'AvianSuite exposes 14 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AvianSuite
provider_slug: aviansuite-com
slug: aviansuite-com-agentic-access
source_filename: aviansuite-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/aviansuite-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 8\n    acting: 6\n  by_consequence:\n    read: 8\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /health/live\n  method: get\n  operationId: live\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/ready\n  method: get\n  operationId: ready\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/root\n  method: get\n  operationId: getRoot\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events\n  method: post\n  operationId: appendEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/events/payloads\n  method: post\n  operationId: getPayloads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/refs/{name}\n  method: get\n  operationId: getRef\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/refs/{name}\n  method: put\n  operationId: putRef\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/verify\n  method: post\n  operationId: verify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/snapshots\n  method: post\n  operationId: createSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/check-root\n  method: get\n  operationId: checkRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/catalog\n  method: get\n  operationId: getCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/catalog/entries\n  method: post\n  operationId: installCatalogEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/catalog/entries/{type}\n\
  \  method: delete\n  operationId: removeCatalogEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/aviansuite-com/agentic-access/aviansuite-com-agentic-access.yml
summary_line: 14 operations · 6 acting
tags:
- Artificial Intelligence
- Agents
- Business Data
- Automation
- Platform
---

---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 4
api_specs:
- filename: port-io-blueprints-api-openapi.yml
  format: yaml
  label: Port Blueprints API
  slug: port-io-blueprints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-blueprints-api-openapi.yml
- filename: port-io-entities-api-openapi.yml
  format: yaml
  label: Port Entities API
  slug: port-io-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-entities-api-openapi.yml
- filename: port-io-action-runs-api-openapi.yml
  format: yaml
  label: Port Action Runs API
  slug: port-io-action-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-action-runs-api-openapi.yml
- filename: port-io-actions-api-openapi.yml
  format: yaml
  label: Port Actions API
  slug: port-io-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-actions-api-openapi.yml
- filename: port-io-ai-api-openapi.yml
  format: yaml
  label: Port AI API
  slug: port-io-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-ai-api-openapi.yml
- filename: port-io-apps-api-openapi.yml
  format: yaml
  label: Port Apps API
  slug: port-io-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-apps-api-openapi.yml
- filename: port-io-audit-api-openapi.yml
  format: yaml
  label: Port Audit API
  slug: port-io-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-audit-api-openapi.yml
- filename: port-io-authentication-authorization-api-openapi.yml
  format: yaml
  label: Port Authentication / Authorization API
  slug: port-io-authentication-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-authentication-authorization-api-openapi.yml
- filename: port-io-folders-api-openapi.yml
  format: yaml
  label: Port Folders API
  slug: port-io-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-folders-api-openapi.yml
- filename: port-io-integrations-api-openapi.yml
  format: yaml
  label: Port Integrations API
  slug: port-io-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-integrations-api-openapi.yml
- filename: port-io-migrations-api-openapi.yml
  format: yaml
  label: Port Migrations API
  slug: port-io-migrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-migrations-api-openapi.yml
- filename: port-io-organization-api-openapi.yml
  format: yaml
  label: Port Organization API
  slug: port-io-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-organization-api-openapi.yml
- filename: port-io-pages-api-openapi.yml
  format: yaml
  label: Port Pages API
  slug: port-io-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-pages-api-openapi.yml
- filename: port-io-scorecard-groups-api-openapi.yml
  format: yaml
  label: Port Scorecard Groups API
  slug: port-io-scorecard-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-scorecard-groups-api-openapi.yml
- filename: port-io-scorecards-api-openapi.yml
  format: yaml
  label: Port Scorecards API
  slug: port-io-scorecards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-scorecards-api-openapi.yml
- filename: port-io-teams-api-openapi.yml
  format: yaml
  label: Port Teams API
  slug: port-io-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-teams-api-openapi.yml
- filename: port-io-users-api-openapi.yml
  format: yaml
  label: Port Users API
  slug: port-io-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-users-api-openapi.yml
- filename: port-io-webhook-api-openapi.yml
  format: yaml
  label: Port Webhook API
  slug: port-io-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-webhook-api-openapi.yml
consequence_counts:
  read: 4
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Port Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Port exposes 8 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Port
provider_slug: port-io
slug: port-io-agentic-access
source_filename: port-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/port-io-blueprints-api-openapi.yml, openapi/port-io-entities-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 4\n    connected: 4\n  by_consequence:\n    write: 4\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/blueprints\n  method: post\n  operationId: createBlueprint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/blueprints\n  method: get\n  operationId: listBlueprints\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/blueprints/{blueprint_identifier}/entities\n  method: post\n  operationId: createEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/blueprints/{blueprint_identifier}/entities\n  method: get\n  operationId: listEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/blueprints/{blueprint_identifier}/entities/{entity_identifier}\n  method: get\n  operationId: getEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /v1/blueprints/{blueprint_identifier}/entities/{entity_identifier}\n  method: patch\n  operationId: updateEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/blueprints/{blueprint_identifier}/entities/{entity_identifier}\n  method: delete\n  operationId: deleteEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/entities/search\n  method: post\n  operationId: searchEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/port-io/agentic-access/port-io-agentic-access.yml
summary_line: 8 operations · 4 acting
tags:
- Internal Developer Portal
- Service Catalog
- Self-Service Actions
- Platform Engineering
- Scorecards
- Developer Experience
- Developer Portal
---

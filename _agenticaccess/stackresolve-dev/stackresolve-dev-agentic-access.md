---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 9
api_specs:
- filename: stackresolve-dev-account-api-openapi.yml
  format: yaml
  label: stackresolve-dev Account API
  slug: stackresolve-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stackresolve-dev/openapi/stackresolve-dev-account-api-openapi.yml
- filename: stackresolve-dev-audit-api-openapi.yml
  format: yaml
  label: stackresolve-dev Audit API
  slug: stackresolve-dev-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stackresolve-dev/openapi/stackresolve-dev-audit-api-openapi.yml
- filename: stackresolve-dev-company-api-openapi.yml
  format: yaml
  label: stackresolve-dev Company API
  slug: stackresolve-dev-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stackresolve-dev/openapi/stackresolve-dev-company-api-openapi.yml
- filename: stackresolve-dev-compare-api-openapi.yml
  format: yaml
  label: stackresolve-dev Compare API
  slug: stackresolve-dev-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stackresolve-dev/openapi/stackresolve-dev-compare-api-openapi.yml
- filename: stackresolve-dev-competitors-api-openapi.yml
  format: yaml
  label: stackresolve-dev Competitors API
  slug: stackresolve-dev-competitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stackresolve-dev/openapi/stackresolve-dev-competitors-api-openapi.yml
- filename: stackresolve-dev-find-tools-api-openapi.yml
  format: yaml
  label: stackresolve-dev Find Tools API
  slug: stackresolve-dev-find-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stackresolve-dev/openapi/stackresolve-dev-find-tools-api-openapi.yml
- filename: stackresolve-dev-plans-api-openapi.yml
  format: yaml
  label: stackresolve-dev Plans API
  slug: stackresolve-dev-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stackresolve-dev/openapi/stackresolve-dev-plans-api-openapi.yml
- filename: stackresolve-dev-pricing-api-openapi.yml
  format: yaml
  label: stackresolve-dev Pricing API
  slug: stackresolve-dev-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stackresolve-dev/openapi/stackresolve-dev-pricing-api-openapi.yml
- filename: stackresolve-dev-profile-api-openapi.yml
  format: yaml
  label: stackresolve-dev Profile API
  slug: stackresolve-dev-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stackresolve-dev/openapi/stackresolve-dev-profile-api-openapi.yml
- filename: stackresolve-dev-registry-api-openapi.yml
  format: yaml
  label: stackresolve-dev Registry API
  slug: stackresolve-dev-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stackresolve-dev/openapi/stackresolve-dev-registry-api-openapi.yml
- filename: stackresolve-dev-research-api-openapi.yml
  format: yaml
  label: stackresolve-dev Research API
  slug: stackresolve-dev-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stackresolve-dev/openapi/stackresolve-dev-research-api-openapi.yml
- filename: stackresolve-dev-search-api-openapi.yml
  format: yaml
  label: stackresolve-dev Search API
  slug: stackresolve-dev-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stackresolve-dev/openapi/stackresolve-dev-search-api-openapi.yml
consequence_counts:
  read: 9
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Stackresolve Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'stackresolve-dev exposes 12 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: stackresolve-dev
provider_slug: stackresolve-dev
slug: stackresolve-dev-agentic-access
source_filename: stackresolve-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/stackresolve-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 9\n    acting: 3\n  by_consequence:\n    read: 9\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/audit\n  method: get\n  operationId: audit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/registry\n  method: get\n  operationId: listRegistry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profile/{slug}\n  method: get\n  operationId:\
  \ getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/find-tools\n  method: post\n  operationId: findTools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/compare\n  method: post\n  operationId: compare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/company\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/plans\n  method: get\n  operationId: getPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/competitors\n  method: get\n  operationId: findCompetitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research\n  method: post\n  operationId: research\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/stackresolve-dev/agentic-access/stackresolve-dev-agentic-access.yml
summary_line: 12 operations · 3 acting
tags:
- AI Agents
- Software Registry
- Web Intelligence
- API Platform
- Developer Tools
---

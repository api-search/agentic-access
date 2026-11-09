---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 12
api_specs:
- filename: basile-cc-enrichissement-api-openapi.yml
  format: yaml
  label: Basile Enrichissement API
  slug: basile-cc-enrichissement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basile-cc/openapi/basile-cc-enrichissement-api-openapi.yml
- filename: basile-cc-entreprises-api-openapi.yml
  format: yaml
  label: Basile Entreprises API
  slug: basile-cc-entreprises-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basile-cc/openapi/basile-cc-entreprises-api-openapi.yml
- filename: basile-cc-personnes-api-openapi.yml
  format: yaml
  label: Basile Personnes API
  slug: basile-cc-personnes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basile-cc/openapi/basile-cc-personnes-api-openapi.yml
- filename: basile-cc-suggestions-api-openapi.yml
  format: yaml
  label: Basile Suggestions API
  slug: basile-cc-suggestions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basile-cc/openapi/basile-cc-suggestions-api-openapi.yml
consequence_counts:
  read: 12
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Basile Cc Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Basile exposes 16 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Basile
provider_slug: basile-cc
slug: basile-cc-agentic-access
source_filename: basile-cc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/original.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 12\n    acting: 4\n  by_consequence:\n    read: 12\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /people/find\n  method: post\n  operationId: findPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/export\n  method: post\n  operationId: exportPeople\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/{id}\n  method: get\n  operationId: getPerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{id}/full\n  method: get\n  operationId: getPersonFull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/roles/suggest\n  method: get\n  operationId: suggestRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/cities/suggest\n  method: get\n  operationId: suggestPeopleCities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/find\n  method: post\n  operationId:\
  \ findCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/export\n  method: post\n  operationId: exportCompanies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{id}\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/activity-suggest\n  method: get\n  operationId: suggestActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/legal-form-suggest\n  method:\
  \ get\n  operationId: suggestLegalForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrichment/find\n  method: post\n  operationId: enrichmentFind\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /enrichment/find/{id}\n  method: get\n  operationId: enrichmentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrichment/find/batch\n  method: post\n  operationId: enrichmentFindBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /enrichment/find/batch/{batchId}\n  method: get\n  operationId: enrichmentBatchStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrichment/wallet\n  method: get\n  operationId: enrichmentWallet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/basile-cc/agentic-access/basile-cc-agentic-access.yml
summary_line: 16 operations · 4 acting
tags:
- Company
- B2B
- Data
- Leads
- French
- Software-as-a-Service
---

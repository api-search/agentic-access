---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 7
api_specs:
- filename: audit-domains-account-api-openapi.yml
  format: yaml
  label: audit.domains Account API
  slug: audit-domains-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audit-domains/openapi/audit-domains-account-api-openapi.yml
- filename: audit-domains-appraisals-api-openapi.yml
  format: yaml
  label: audit.domains Appraisals API
  slug: audit-domains-appraisals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audit-domains/openapi/audit-domains-appraisals-api-openapi.yml
- filename: audit-domains-bulk-api-openapi.yml
  format: yaml
  label: audit.domains Bulk API
  slug: audit-domains-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audit-domains/openapi/audit-domains-bulk-api-openapi.yml
- filename: audit-domains-machine-api-openapi.yml
  format: yaml
  label: audit.domains Machine API
  slug: audit-domains-machine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audit-domains/openapi/audit-domains-machine-api-openapi.yml
- filename: audit-domains-sales-api-openapi.yml
  format: yaml
  label: audit.domains Sales API
  slug: audit-domains-sales-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audit-domains/openapi/audit-domains-sales-api-openapi.yml
consequence_counts:
  physical: 1
  read: 7
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Audit Domains Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/machine/resolve
operation_count: 10
overview: 'audit.domains exposes 10 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: audit.domains
provider_slug: audit-domains
slug: audit-domains-agentic-access
source_filename: audit-domains-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/audit-domains-openapi-machine.json, openapi/audit-domains-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 7\n    acting: 3\n  by_consequence:\n    read: 7\n    physical: 1\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/machine/resolve\n  method: get\n  operationId: machineTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/machine/resolve\n  method: post\n  operationId: machineResolve\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/appraise\n  method: post\n  operationId: appraiseDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/comps\n  method: get\n  operationId: getComps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/comps\n  method: head\n  operationId: headComps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/bulk\n  method: post\n  operationId: bulkAppraise\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage\n  method: head\n  operationId: headUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sales\n  method: get\n  operationId: searchSales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sales\n  method:\
  \ head\n  operationId: headSales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/audit-domains/agentic-access/audit-domains-agentic-access.yml
summary_line: 10 operations · 3 acting
tags:
- Domain
- Valuation
- Analytics
- Portfolio
---

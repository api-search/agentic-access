---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 9
api_specs:
- filename: denim-openapi-original.json
  format: json
  label: Denim Public API
  slug: denim-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denim/refs/heads/main/openapi/denim-openapi-original.json
consequence_counts:
  read: 9
  safety-critical: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Denim Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/debtor-relationships
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/jobs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/jobs/quote
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/jobs/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/jobs/{job_id}/documents
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/jobs/{job_id}/revert-to-draft
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/payee-relationships
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/payee-relationships/{client_payee_relationship_id}/update-assign-factor
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/jobs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/jobs/{job_id}/document
operation_count: 19
overview: 'Denim exposes 19 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Denim
provider_slug: denim
slug: denim-agentic-access
source_filename: denim-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/denim-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 9\n    acting: 10\n  by_consequence:\n    read: 9\n    safety-critical: 10\n  human_in_the_loop_required: 10\noperations:\n- path: /api/v1/companies\n  method: get\n  operationId: AxlePayWeb.Api.V1.CompanyController.index (2)\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/factors\n  method: get\n  operationId: AxlePayWeb.Api.V1.FactoringCompanyController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/debtor-relationships\n  method: get\n  operationId: AxlePayWeb.Api.V1.ClientDebtorRelationshipController.index (2)\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/debtor-relationships\n  method: post\n  operationId: AxlePayWeb.Api.V1.ClientDebtorRelationshipController.create (2)\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/jobs\n  method: get\n  operationId: AxlePayWeb.Api.V1.JobController.index (2)\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/jobs\n  method: post\n  operationId: AxlePayWeb.Api.V1.JobController.create (2)\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/jobs/quote\n  method: post\n  operationId: AxlePayWeb.Api.V1.JobController.get_quote\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/jobs/{id}\n  method: delete\n  operationId: AxlePayWeb.Api.V1.JobController.delete (2)\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/jobs/{id}\n  method: get\n  operationId: AxlePayWeb.Api.V1.JobController.show (2)\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jobs/{job_id}/documents\n  method: post\n  operationId: Elixir.AxlePayWeb.Api.V1.Job.DocumentController.create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/jobs/{job_id}/revert-to-draft\n\
  \  method: post\n  operationId: AxlePayWeb.Api.V1.JobController.revert_to_draft (2)\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/payee-relationships\n  method: get\n  operationId: AxlePayWeb.Api.V1.ClientPayeeRelationshipController.index (2)\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/payee-relationships\n  method: post\n  operationId: AxlePayWeb.Api.V1.ClientPayeeRelationshipController.create (2)\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/payee-relationships/{client_payee_relationship_id}/update-assign-factor\n  method: post\n  operationId: AxlePayWeb.Api.V1.ClientPayeeRelationshipController.update_assign_factor (2)\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/transactions\n  method: get\n  operationId: AxlePayWeb.Api.V1.TransactionController.index (2)\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/jobs\n  method: get\n  operationId: AxlePayWeb.Api.V2.JobController.index\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/jobs\n  method: post\n  operationId: AxlePayWeb.Api.V2.JobController.create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/jobs/{job_id}\n  method: get\n  operationId: AxlePayWeb.Api.V2.JobController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/jobs/{job_id}/document\n  method: post\n  operationId: AxlePayWeb.Api.V2.JobController.create_document\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/denim/refs/heads/main/agentic-access/denim-agentic-access.yml
summary_line: 19 operations · 10 acting · 10 human-in-the-loop
tags:
- Company
- Freight
- Factoring
- Payments
- Logistics
- Trucking
- Fintech
- Back Office
---

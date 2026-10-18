---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 5
api_specs:
- filename: plangrid-batch-api-openapi.yml
  format: yaml
  label: PlanGrid Batch API
  slug: plangrid-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plangrid/refs/heads/main/openapi/plangrid-batch-api-openapi.yml
- filename: plangrid-me-api-openapi.yml
  format: yaml
  label: PlanGrid Me API
  slug: plangrid-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plangrid/refs/heads/main/openapi/plangrid-me-api-openapi.yml
- filename: plangrid-oauth-api-openapi.yml
  format: yaml
  label: PlanGrid OAuth API
  slug: plangrid-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plangrid/refs/heads/main/openapi/plangrid-oauth-api-openapi.yml
- filename: plangrid-projects-api-openapi.yml
  format: yaml
  label: PlanGrid Projects API
  slug: plangrid-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plangrid/refs/heads/main/openapi/plangrid-projects-api-openapi.yml
- filename: plangrid-rate-limits-api-openapi.yml
  format: yaml
  label: PlanGrid Rate Limits API
  slug: plangrid-rate-limits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plangrid/refs/heads/main/openapi/plangrid-rate-limits-api-openapi.yml
consequence_counts:
  physical: 1
  read: 5
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Plangrid Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /batch
operation_count: 8
overview: 'PlanGrid exposes 8 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PlanGrid
provider_slug: plangrid
slug: plangrid-agentic-access
source_filename: plangrid-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/plangrid-no-api-explorer-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 3\n    connected: 5\n  by_consequence:\n    physical: 1\n    read: 5\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /batch\n  method: post\n  operationId: send-batch-request\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me\n  method: get\n  operationId:\
  \ get-user-profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/authorize\n  method: get\n  operationId: retrieve-authorization-code\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/token\n  method: post\n  operationId: retrieve-access-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects\n  method: post\n  operationId: create-project\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects\n  method: get\n  operationId: list-all-projects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_uid}/rfis2/{rfi_uid}/return_messages\n  method: get\n  operationId: get-rfi-return-message-in-a-project\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rate_limits\n  method: get\n  operationId: retrieve-rate-limits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plangrid/refs/heads/main/agentic-access/plangrid-agentic-access.yml
summary_line: 8 operations · 3 acting
tags:
- Company
- Enterprise
- Construction
- Construction Technology
- Project Management
- Field Reports
- Documents
- RFIs
- REST API
- Autodesk
---

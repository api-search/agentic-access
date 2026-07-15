---
acting_count: 327
action_class_counts:
  acting: 327
  connected: 332
api_specs:
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel People API
  slug: deel-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Organizations API
  slug: deel-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Contracts API
  slug: deel-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Time Off API
  slug: deel-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Time Tracking API
  slug: deel-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Payroll API
  slug: deel-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Invoices API
  slug: deel-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Expenses API
  slug: deel-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel EOR API
  slug: deel-eor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Background Checks API
  slug: deel-background-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Immigration API
  slug: deel-immigration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel IT API
  slug: deel-it-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel SCIM API
  slug: deel-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel ATS API
  slug: deel-ats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Accounting API
  slug: deel-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Lookups API
  slug: deel-lookups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Webhooks API
  slug: deel-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel OAuth & Apps API
  slug: deel-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel MCP Server
  slug: deel-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
consequence_counts:
  physical: 20
  read: 332
  safety-critical: 10
  write: 297
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Deel Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /contracts/{contract_id}/terminations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /contracts/{contract_id}/terminations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /timesheets/presets
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /timesheets/presets
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /timesheets/presets/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /timesheets/presets/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /timesheets/presets/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /timesheets/presets/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /timesheets/root-presets
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /timesheets/root-presets
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /contracts/{contract_id}/invitations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /contracts/{contract_id}/invitations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /contracts/{contract_id}/off-cycle-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /contracts/{contract_id}/off-cycle-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoice-adjustments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoice-adjustments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /invoice-adjustments/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /invoice-adjustments/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /invoice-adjustments/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /invoice-adjustments/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoice-adjustments/{id}/reviews
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoice-adjustments/{id}/reviews
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /payouts/auto-withdrawal-setting
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/contractors/methods
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payouts/contractors/methods/{id}
operation_count: 659
overview: 'Deel exposes 659 API operations that an AI agent could call, of which 327 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 332 read, 297 write, 20 physical, and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Deel
provider_slug: deel
slug: deel-agentic-access
source_filename: deel-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/deel-contracts-endpoints-openapi.json, openapi/deel-custom-fields-endpoints-openapi.json,\n  openapi/deel-endpoints-1-openapi.json, openapi/deel-eor-endpoints-openapi.json, openapi/deel-eor-worker-endpoints-openapi.json,\n  openapi/deel-global-payroll-endpoints-openapi.json, openapi/deel-it-endpoints-openapi.json,\n  openapi/deel-platform-endpoints-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 659\n  by_action_class:\n    acting: 327\n    connected: 332\n  by_consequence:\n    write: 297\n    read: 332\n    physical: 20\n    safety-critical: 10\n  human_in_the_loop_required: 10\noperations:\n- path: /contracts/{contract_id}/amendments\n  method: post\n  operationId: create-contract-amendment\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/amendments\n  method: get\n  operationId: get-contract-amendments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/documents\n  method: post\n  operationId: create-contract-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/invite\n  method: get\n  operationId: get-contract-invite\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/preview\n  method: get\n  operationId: get-contract-preview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/invitations\n  method: delete\n  operationId: get-contract-invitations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/invitations\n  method: post\n  operationId: create-contract-invitation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/payment_cycles\n  method: get\n  operationId: get-contract-payment-cycles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/signatures\n  method: post\n  operationId: create-contract-signature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}\n  method: patch\n  operationId: update-ic-contract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}\n  method: get\n  operationId: get-contract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts\n  method: post\n  operationId: create-ic-contract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts\n  method: get\n  operationId: get-contracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice-adjustments\n  method:\
  \ post\n  operationId: create-invoice-adjustment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoice-adjustments\n  method: get\n  operationId: get-invoice-adjustments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice-adjustments/{id}\n  method: delete\n  operationId: delete-invoice-adjustment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /invoice-adjustments/{id}\n  method: get\n  operationId: get-invoice-adjustment-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice-adjustments/{id}\n  method: patch\n  operationId: update-invoice-adjustment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/invoice-adjustments\n  method: get\n  operationId: get-contract-invoice-adjustments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice-adjustments/{id}/reviews\n\
  \  method: post\n  operationId: create-invoice-adjustment-review\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/milestones\n  method: post\n  operationId: create-contract-milestone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/milestones\n  method: get\n  operationId: get-contract-milestones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /contracts/{contract_id}/milestones/{milestone_id}\n  method: delete\n  operationId: delete-contract-milestone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/milestones/{milestone_id}\n  method: get\n  operationId: get-contract-milestone-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/off-cycle-payments\n  method: post\n  operationId: create-contract-off-cycle-payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/off-cycle-payments\n  method: get\n  operationId: get-contract-off-cycle-payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/off-cycle-payments/{id}\n  method: get\n  operationId: get-contract-off-cycle-payment-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timesheets/presets\n  method: post\n  operationId: create-timesheets-preset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /timesheets/root-presets\n  method: post\n  operationId: create-root-timesheets-preset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /timesheets/presets/{id}\n  method: delete\n  operationId: delete-timesheets-preset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /timesheets/presets/{id}\n  method: get\n  operationId: get-timesheets-preset-by-id\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timesheets/presets/{id}\n  method: patch\n  operationId: update-timesheets-preset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /contracts/{contract_id}/timesheets/presets\n  method: get\n  operationId: get-contract-timesheets-presets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/tasks\n  method: post\n  operationId: create-contract-task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/tasks\n  method: get\n  operationId: get-contract-tasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/tasks/{task_id}\n  method: delete\n  operationId: delete-contract-task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/tasks/{task_id}/reviews\n  method: post\n  operationId: create-contract-task-review\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/terminations\n  method: delete\n  operationId: delete-contract-termination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/terminations\n  method: post\n  operationId: create-contract-termination\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /timesheets\n\
  \  method: post\n  operationId: create-timesheet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /timesheets\n  method: get\n  operationId: get-timesheets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/timesheets\n  method: get\n  operationId: get-contract-timesheets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timesheets/{id}\n  method: get\n  operationId: get-timesheet-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /timesheets/{id}\n  method: patch\n  operationId: update-timesheet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /timesheets/{id}/reviews\n  method: post\n  operationId: create-timesheet-review\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/custom_fields/{id}\n  method: delete\n  operationId: delete-contract-custom-field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/custom_fields/{id}\n  method: get\n  operationId: get-custom-field\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/custom_fields\n  method: get\n  operationId: get-contract-custom-fields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/custom_fields\n  method: put\n  operationId: put-contract-custom-field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/{worker_id}/custom_fields/{id}\n\
  \  method: delete\n  operationId: delete-person-custom-field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/custom_fields/{id}\n  method: get\n  operationId: get-person-custom-field\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/custom_fields\n  method: get\n  operationId: get-custom-fields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{worker_id}/custom_fields\n  method: get\n  operationId: get-person-custom-fields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{worker_id}/custom_fields\n  method: put\n  operationId: put-person-custom-field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hris/organization_structures\n  method: post\n  operationId: create-organization-structure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hris/organization_structures\n  method: get\n  operationId: get-organization-structures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /hris/organization_structures/external/{external_id}\n  method: delete\n  operationId: delete-organization-structure-by-external-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hris/organization_structures/external/{external_id}\n  method: get\n  operationId: get-organization-structure-by-external-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hris/organization_structures/external/{external_id}\n  method: patch\n  operationId: update-organization-structure-by-external-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hris/organization_structures/{hrisOrgStr_id}\n  method: delete\n  operationId: delete-organization-structure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hris/organization_structures/{hrisOrgStr_id}\n  method: get\n  operationId: get-organization-structure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hris/organization_structures/{hrisOrgStr_id}\n  method: patch\n  operationId: update-organization-structure\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hris/organization-structures/teams/{team_id}/custom-fields\n  method: get\n  operationId: get-team-custom-fields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hris/organization-structures/teams/{team_id}/custom-fields\n  method: patch\n  operationId: update-team-custom-fields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/{id}/department\n  method: put\n  operationId: update-person-department\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pwac\n  method: post\n  operationId: create-person-without-contract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people\n  method: get\n  operationId: get-people\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{hris_profile_id}\n  method: get\n  operationId: get-person-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{id}/working-location\n  method: put\n  operationId: update-person-working-location\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/{worker_id}/personal\n  method: get\n  operationId: get-person-personal-info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{worker_id}/personal\n  method: patch\n  operationId: update-person-personal-info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /people/external/{worker_id}/personal\n  method: get\n  operationId: get-person-personal-info-external-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/external/{worker_id}/personal\n  method: patch\n  operationId: update-person-personal-info-external-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hris/positions/apply_changes\n  method: post\n  operationId: apply-position-changes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hris/positions/profile/{hrisProfileId}\n  method: get\n  operationId: get-positions-by-profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time_offs/review\n  method: post\n  operationId: review-time-off-request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /time_offs/{time_off_id}\n  method: delete\n  operationId: delete-time-off-request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /time_offs/{time_off_id}\n  method: patch\n  operationId: update-time-off-request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /time_offs\n  method: post\n  operationId: create-time-off-request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /time_offs/global-payroll/sync\n  method: post\n  operationId: sync-time-off-global-payroll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /time_offs/profile/{hris_profile_id}/entitlements\n  method: get\n  operationId: get-time-off-entitlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time_offs/time-off-events\n  method: get\n  operationId: get-time-off-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time_offs/dailies\n  method: get\n  operationId: get-time-off-dailies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time_offs/profile/{hris_profile_id}/policies\n  method: get\n  operationId: get-time-off-policies\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time_offs/profile/{hris_profile_id}\n  method: get\n  operationId: get-time-off-profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time_offs/policy-validation-templates\n  method: get\n  operationId: get-time-off-policy-validation-templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time_offs/validate\n  method: post\n  operationId: validate-time-off\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /Users\n  method: get\n  operationId: get-users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Users/{hrisProfileOid}\n  method: get\n  operationId: get-user-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Users/.search\n  method: post\n  operationId: search-users\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hris/worker_relations/profile/{hrisProfileOid}/child\n  method: put\n  operationId: add-worker-relation-child\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hris/worker_relations/profile/external/{profileId}/parent\n  method: put\n  operationId: add-worker-relation-parent-by-external-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hris/worker_relations/profile/{hrisProfileOid}/parent\n  method: put\n  operationId: add-worker-relation-parent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hris/worker_relations/profile\n\
  \  method: post\n  operationId: create-worker-relation-profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hris/worker_relations/profile/external/{profileId}/child\n  method: put\n  operationId: add-worker-relation-child-by-external-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hris/worker_relations/types\n  method: post\n  operationId: create-worker-relation-type\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hris/worker_relations/types\n  method: get\n  operationId: get-worker-relation-types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hris/worker_relations/profile/external\n  method: post\n  operationId: create-worker-relation-profile-by-external-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hris/worker_relations/profile/{hrisProfileOid}\n  method: delete\n  operationId: delete-worker-relation-profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hris/worker_relations/profile/{hrisProfileOid}\n  method: get\n  operationId: get-worker-relation-profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hris/worker_relations/profile/external/{profileId}\n  method: delete\n  operationId: delete-worker-relation-profile-by-external-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hris/worker_relations/profile/external/{profileId}\n  method: get\n  operationId: get-worker-relation-profile-by-external-id\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: option\n\n# --- truncated at 32 KB (196 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/agentic-access/deel-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/agentic-access/deel-agentic-access.yml
summary_line: 659 operations · 327 acting · 10 human-in-the-loop
tags:
- HR
- Payroll
- Global Hiring
- EOR
- Contractors
- Compliance
- SCIM
---

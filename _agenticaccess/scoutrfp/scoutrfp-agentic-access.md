---
acting_count: 113
action_class_counts:
  acting: 113
  connected: 95
api_specs:
- filename: scoutrfp-suppliers-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Suppliers API
  slug: workday-strategic-sourcing-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-suppliers-v1-openapi.json
- filename: scoutrfp-events-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Events API
  slug: workday-strategic-sourcing-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-events-v1-openapi.json
- filename: scoutrfp-reports-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Reports API
  slug: workday-strategic-sourcing-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-reports-v1-openapi.json
- filename: scoutrfp-contracts-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Contracts API
  slug: workday-strategic-sourcing-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-contracts-v1-openapi.json
- filename: scoutrfp-projects-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Projects API
  slug: workday-strategic-sourcing-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-projects-v1-openapi.json
- filename: scoutrfp-payments-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Payments API
  slug: workday-strategic-sourcing-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-payments-v1-openapi.json
- filename: scoutrfp-fields-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Fields API
  slug: workday-strategic-sourcing-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-fields-v1-openapi.json
- filename: scoutrfp-awards-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Awards API
  slug: workday-strategic-sourcing-awards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-awards-v1-openapi.json
- filename: scoutrfp-attachments-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Attachments API
  slug: workday-strategic-sourcing-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-attachments-v1-openapi.json
- filename: scoutrfp-spend_categories-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Spend Categories API
  slug: workday-strategic-sourcing-spend-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-spend_categories-v1-openapi.json
- filename: scoutrfp-scim-v2-openapi.json
  format: json
  label: Workday Strategic Sourcing - SCIM (Users) API
  slug: workday-strategic-sourcing-scim-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-scim-v2-openapi.json
consequence_counts:
  physical: 31
  read: 95
  write: 82
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Scoutrfp Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events/{event_external_id}/relationships/supplier_companies/external_id
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /events/{event_external_id}/relationships/supplier_companies/external_id
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events/{event_external_id}/relationships/supplier_contacts/external_id
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /events/{event_external_id}/relationships/supplier_contacts/external_id
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events/{event_id}/relationships/supplier_companies
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /events/{event_id}/relationships/supplier_companies
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events/{event_id}/relationships/supplier_contacts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /events/{event_id}/relationships/supplier_contacts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment_currencies
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /payment_currencies/{external_id}/external_id
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payment_currencies/{external_id}/external_id
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /payment_currencies/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payment_currencies/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment_terms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /payment_terms/{external_id}/external_id
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payment_terms/{external_id}/external_id
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /payment_terms/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payment_terms/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment_types
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /payment_types/{external_id}/external_id
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payment_types/{external_id}/external_id
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /payment_types/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payment_types/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /projects/{project_external_id}/relationships/supplier_companies/external_id
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /projects/{project_external_id}/relationships/supplier_companies/external_id
operation_count: 208
overview: 'Scout RFP (Workday Strategic Sourcing) exposes 208 API operations that an AI agent could call, of which 113 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 95 read, 82 write, and 31 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Scout RFP (Workday Strategic Sourcing)
provider_slug: scoutrfp
slug: scoutrfp-agentic-access
source_filename: scoutrfp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/scoutrfp-attachments-v1-openapi.json, openapi/scoutrfp-awards-v1-openapi.json,\n  openapi/scoutrfp-contracts-v1-openapi.json, openapi/scoutrfp-events-v1-openapi.json, openapi/scoutrfp-fields-v1-openapi.json,\n  openapi/scoutrfp-payments-v1-openapi.json, openapi/scoutrfp-projects-v1-openapi.json, openapi/scoutrfp-reports-v1-openapi.json,\n  openapi/scoutrfp-scim-v2-openapi.json, openapi/scoutrfp-spend_categories-v1-openapi.json,\n  openapi/scoutrfp-suppliers-v1-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 208\n  by_action_class:\n    connected: 95\n    acting: 113\n  by_consequence:\n    read: 95\n    write: 82\n    physical: 31\n  human_in_the_loop_required: 0\noperations:\n\
  - path: /attachments\n  method: get\n  operationId: List Attachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attachments\n  method: post\n  operationId: Create an Attachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attachments/{id}\n  method: get\n  operationId: Get an Attachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attachments/{id}\n  method: patch\n  operationId: Update an Attachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attachments/{external_id}/external_id\n  method: get\n  operationId: Get an Attachment by External ID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attachments/{external_id}/external_id\n  method: patch\n  operationId: Update an Attachment by External ID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /awards\n  method: get\n  operationId: List Awards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /awards/{award_id}/award_line_items\n  method: get\n  operationId: List Award Line Items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /award_line_items/{id}\n  method: get\n  operationId: Get an Award Line Item\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts\n  method: get\n  operationId: List Contracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts\n  method: post\n  operationId: Create a Contract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /contracts/{id}\n  method: get\n  operationId: Get a Contract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{id}\n  method: patch\n  operationId: Update a Contract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{id}\n  method: delete\n  operationId: Delete a Contract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{external_id}/external_id\n\
  \  method: get\n  operationId: Get a Contract by External ID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{external_id}/external_id\n  method: patch\n  operationId: Update a Contract by External ID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{external_id}/external_id\n  method: delete\n  operationId: Delete a Contract by External ID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/describe\n\
  \  method: get\n  operationId: Describe Contract object\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contract_types\n  method: get\n  operationId: List Contract Types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contract_types\n  method: post\n  operationId: Create a Contract Type\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contract_types/{id}\n  method: get\n  operationId: Get a Contract Type\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /contract_types/{id}\n  method: patch\n  operationId: Update a Contract Type\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contract_types/{id}\n  method: delete\n  operationId: Delete a Contract Type\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contract_types/{external_id}/external_id\n  method: get\n  operationId: Get a Contract Type by External ID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /contract_types/{external_id}/external_id\n  method: patch\n  operationId: Update a Contract Type by External ID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contract_types/{external_id}/external_id\n  method: delete\n  operationId: Delete a Contract Type by External ID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event_templates\n  method: get\n  operationId: List Event Templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /event_templates/{id}\n  method: get\n  operationId: Get an Event Template\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: List Events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: post\n  operationId: Create an Event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{id}\n  method: get\n  operationId: Get an Event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /events/{id}\n  method: patch\n  operationId: Update an Event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{id}\n  method: delete\n  operationId: Delete an Event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/describe\n  method: get\n  operationId: Describe Event Object\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{event_id}/worksheets\n  method: get\n  operationId:\
  \ List Worksheets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{event_id}/worksheets/{id}\n  method: get\n  operationId: Get a Worksheet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /worksheets/describe\n  method: get\n  operationId: Describe Worksheet object\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{event_id}/worksheets/{worksheet_id}/line_items\n  method: get\n  operationId: List Line Items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{event_id}/worksheets/{worksheet_id}/line_items\n  method: post\n  operationId: Create a Line\
  \ Item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{event_id}/worksheets/{worksheet_id}/line_items/bulk\n  method: post\n  operationId: Bulk Create Line Items\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{event_id}/worksheets/{worksheet_id}/line_items/{id}\n  method: get\n  operationId: Get a Line Item\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{event_id}/worksheets/{worksheet_id}/line_items/{id}\n\
  \  method: patch\n  operationId: Update a Line Item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{event_id}/worksheets/{worksheet_id}/line_items/{id}\n  method: delete\n  operationId: Delete a Line Item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{event_id}/relationships/supplier_companies\n  method: post\n  operationId: Add Suppliers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{event_id}/relationships/supplier_companies\n  method: delete\n  operationId: Remove Suppliers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{event_external_id}/relationships/supplier_companies/external_id\n  method: post\n  operationId: Add Suppliers using External IDs\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{event_external_id}/relationships/supplier_companies/external_id\n  method: delete\n  operationId: Remove Suppliers using External IDs\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{event_id}/relationships/supplier_contacts\n  method: post\n  operationId: Add Suppliers using Contacts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /events/{event_id}/relationships/supplier_contacts\n  method: delete\n  operationId: Remove Suppliers using Contacts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{event_external_id}/relationships/supplier_contacts/external_id\n  method: post\n  operationId: Add Suppliers using Contacts External IDs\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{event_external_id}/relationships/supplier_contacts/external_id\n\
  \  method: delete\n  operationId: Remove Suppliers using Contacts External IDs\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{event_id}/bids\n  method: get\n  operationId: List Bids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bids/{id}\n  method: get\n  operationId: Get a Bid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bids/describe\n  method: get\n  operationId: Describe Bid object\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bids/{bid_id}/bid_line_items\n  method: get\n  operationId: List Bid Line Items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bid_line_items/{id}\n  method: get\n  operationId: Get a Bid Line Item\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bid_line_items\n  method: get\n  operationId: List All Bid Line Items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bid_line_items/describe\n  method: get\n  operationId: Describe Bid Line Item Object\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /fields\n  method: get\n  operationId: List Fields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fields\n  method: post\n  operationId: Create a Field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fields/{id}\n  method: get\n  operationId: Get a Field\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fields/{id}\n  method: patch\n  operationId: Update a Field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fields/{id}\n  method: delete\n  operationId: Delete a Field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fields/{field_id}/field_options\n  method: get\n  operationId: List Field Options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /field_options\n  method: post\n  operationId: Create a Field Option\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /field_options/{id}\n  method: patch\n  operationId: Update a Field Option\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /field_options/{id}\n  method: delete\n  operationId: Delete a Field Option\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /field_groups\n  method: get\n  operationId: List Field Groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /field_groups\n  method: post\n\
  \  operationId: Create a Field Group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /field_groups/{id}\n  method: get\n  operationId: Get a Field Group\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /field_groups/{id}\n  method: patch\n  operationId: Update a Field Group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /field_groups/{id}\n  method: delete\n  operationId: Delete a Field Group\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_terms\n  method: get\n  operationId: List Payment Terms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment_terms\n  method: post\n  operationId: Create a Payment Term\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_terms/{id}\n  method: patch\n  operationId: Update a Payment Term\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_terms/{id}\n  method: delete\n  operationId: Delete a Payment Term\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_terms/{external_id}/external_id\n  method: patch\n  operationId: Update a Payment Term by External ID\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_terms/{external_id}/external_id\n  method: delete\n  operationId: Delete a Payment Term by External ID\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_types\n  method: get\n  operationId: List Payment Types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment_types\n  method: post\n  operationId: Create a Payment Type\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_types/{id}\n  method: patch\n  operationId: Update a Payment Type\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_types/{id}\n  method: delete\n  operationId: Delete a Payment Type\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_types/{external_id}/external_id\n  method: patch\n  operationId: Update a Payment Type by External ID\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_types/{external_id}/external_id\n  method: delete\n  operationId: Delete a Payment Type by External ID\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_currencies\n\
  \  method: get\n  operationId: List Payment Currencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment_currencies\n  method: post\n  operationId: Create a Payment Currency\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_currencies/{id}\n  method: patch\n  operationId: Update a Payment Currency\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /payment_currencies/{id}\n  method: delete\n  operationId: Delete a Payment Currency\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_currencies/{external_id}/external_id\n  method: patch\n  operationId: Update a Payment Currency by External ID\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_currencies/{external_id}/external_id\n  method: delete\n\
  \  operationId: Delete a Payment Currency by External ID\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects\n  method: get\n  operationId: List Projects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: post\n  operationId: Create a Project\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{id}\n  method: get\n  operationId: Get\
  \ a Project\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{id}\n  method: patch\n  operationId: Update a Project\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{id}\n  method: delete\n  operationId: Delete a Project\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{external_id}/external_id\n  method: get\n  operationId: Get a Project by External ID\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{external_id}/external_id\n  method: patch\n  operationId: Update a Project by External ID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{external_id}/external_id\n  method: delete\n  operationId: Delete a Project by External ID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/describe\n  method: get\n  operationId: Describe Project object\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/relationships/supplier_companies\n  method: post\n  operationId: Add Suppliers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/relationships/supplier_companies\n  method: delete\n  operationId: Remove Suppliers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /projects/{project_external_id}/relationships/s\n\n# --- truncated at 32 KB (63 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/agentic-access/scoutrfp-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/agentic-access/scoutrfp-agentic-access.yml
summary_line: 208 operations · 113 acting
tags:
- Company
- Enterprise
- Procurement
- Strategic Sourcing
- Supplier Management
- Spend Management
- RFP
- Contracts
- SCIM
- JSON:API
---

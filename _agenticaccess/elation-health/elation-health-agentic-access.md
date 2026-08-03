---
acting_count: 455
action_class_counts:
  acting: 455
  connected: 391
api_specs:
- filename: elation-api-authentication.json
  format: json
  label: Elation OAuth API
  slug: oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-api-authentication.json
- filename: elation-patient-profile-api.json
  format: json
  label: Elation Patient Profile API
  slug: patient-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-patient-profile-api.json
- filename: elation-visit-notes-api.json
  format: json
  label: Elation Visit Notes API
  slug: visit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-visit-notes-api.json
- filename: elation-patient-document-api.json
  format: json
  label: Elation Patient Document API
  slug: patient-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-patient-document-api.json
- filename: elation-orders-api.json
  format: json
  label: Elation Orders API
  slug: orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-orders-api.json
- filename: elation-scheduling-api.json
  format: json
  label: Elation Scheduling API
  slug: scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-scheduling-api.json
- filename: elation-billing-api.json
  format: json
  label: Elation Billing API
  slug: billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-billing-api.json
- filename: elation-insurance-api.json
  format: json
  label: Elation Insurance API
  slug: insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-insurance-api.json
- filename: elation-premium-patient-insurance-api.json
  format: json
  label: Elation Patient Insurance API (Premium) & Eligibility
  slug: patient-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-premium-patient-insurance-api.json
- filename: elation-practice-api.json
  format: json
  label: Elation Practice API
  slug: practice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-practice-api.json
- filename: elation-user-management-api.json
  format: json
  label: Elation User Management API
  slug: user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-user-management-api.json
- filename: elation-messaging-api.json
  format: json
  label: Elation Messaging API
  slug: messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-messaging-api.json
- filename: elation-event-subscription-api.json
  format: json
  label: Elation Event Subscription API
  slug: event-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-event-subscription-api.json
- filename: elation-reference-data-api.json
  format: json
  label: Elation Reference Data API
  slug: reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-reference-data-api.json
- filename: elation-care-gaps-api-1.json
  format: json
  label: Elation Care Gaps API
  slug: care-gaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-care-gaps-api-1.json
- filename: elation-elation-import-api.json
  format: json
  label: Elation Import API
  slug: import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-elation-import-api.json
- filename: elation-api-settings.json
  format: json
  label: Elation Health API Settings
  slug: elation-api-settings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-api-settings.json
consequence_counts:
  physical: 87
  read: 391
  write: 368
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Elation Health Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/2.0/cardiac_order_tests/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/2.0/cardiac_order_tests/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/2.0/cardiac_orders/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/2.0/cardiac_orders/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/2.0/cardiac_orders/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/2.0/cardiac_orders/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/2.0/imaging_order_tests/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/2.0/imaging_order_tests/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/2.0/imaging_orders/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/2.0/imaging_orders/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/2.0/imaging_orders/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/2.0/imaging_orders/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/2.0/lab_order_compendiums/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/2.0/lab_order_compendiums/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/2.0/lab_order_compendiums/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/2.0/lab_order_compendiums/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/2.0/lab_order_sets/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/2.0/lab_order_sets/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/2.0/lab_order_sets/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/2.0/lab_order_sets/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/2.0/lab_order_tests/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/2.0/lab_order_tests/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/2.0/lab_orders/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/2.0/lab_orders/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/2.0/lab_orders/{id}/
operation_count: 846
overview: 'Elation Health exposes 846 API operations that an AI agent could call, of which 455 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 391 read, 368 write, and 87 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Elation Health
provider_slug: elation-health
slug: elation-health-agentic-access
source_filename: elation-health-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: generated\nsource: openapi/elation-api-settings.json, openapi/elation-billing-api.json, openapi/elation-care-gaps-api-1.json,\n  openapi/elation-elation-import-api.json, openapi/elation-event-subscription-api.json, openapi/elation-insurance-api.json,\n  openapi/elation-messaging-api.json, openapi/elation-orders-api.json, openapi/elation-patient-document-api.json,\n  openapi/elation-patient-profile-api.json, openapi/elation-practice-api.json, openapi/elation-premium-patient-insurance-api.json,\n  openapi/elation-reference-data-api.json, openapi/elation-scheduling-api.json, openapi/elation-user-management-api.json,\n  openapi/elation-visit-notes-api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 846\n  by_action_class:\n\
  \    acting: 455\n    connected: 391\n  by_consequence:\n    write: 368\n    read: 391\n    physical: 87\n  human_in_the_loop_required: 0\noperations:\n- path: /patients/:id/\n  method: put\n  operationId: update-patient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patients/{id}\n  method: get\n  operationId: get-patient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /problems/\n  method: get\n  operationId: list-problems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /problems/\n  method: post\n  operationId: create-problem\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patients/{id}/\n  method: delete\n  operationId: delete-patient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patients/{id}/\n  method: patch\n  operationId: update-patient-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointments/{id}/\n  method: delete\n\
  \  operationId: delete-event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointments/{id}/\n  method: get\n  operationId: get-event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointments/{id}/\n  method: put\n  operationId: update-appointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointments/{id}/\n  method: patch\n  operationId: update-event\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /problems/{id}/\n  method: get\n  operationId: get-problem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /problems/{id}/\n  method: delete\n  operationId: delete-problem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /problems/{id}/\n  method: patch\n  operationId: patch-problem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointments/\n  method: post\n  operationId: create-event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointments/\n  method: get\n  operationId: testinput\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vitals/{id}/\n  method: get\n  operationId: get-vital\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /physicians/\n  method: get\n  operationId: find-physicians\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /medications/\n  method: get\n  operationId: find-medications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /medications/\n  method: post\n  operationId: create-medication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /allergies/{id}/\n  method: put\n  operationId: update-allergy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /allergies/{id}/\n  method: get\n  operationId: get-allergy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /allergies/{id}/\n  method: delete\n  operationId: delete-allergy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ccda/\n  method: post\n  operationId: create-ccda\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /immunizations/{id}/\n  method: delete\n  operationId:\
  \ delete-immunization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /immunizations/{id}/\n  method: get\n  operationId: get-immunization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /family_histories/{id}/\n  method: get\n  operationId: get-family-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /family_histories/{id}/\n  method: delete\n  operationId: delete-family-history\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /histories/\n  method: post\n  operationId: create-history\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /histories/\n  method: get\n  operationId: find-histories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /allergies/\n  method: get\n  operationId: find-allergies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /allergies/\n  method: post\n  operationId: create-allergy\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /immunizations/\n  method: get\n  operationId: find-immunizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /immunizations/\n  method: post\n  operationId: create-immunization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/{id}/\n  method: get\n  operationId: get-bill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /bills/{id}/\n  method: patch\n  operationId: patch-bill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/{id}/\n  method: delete\n  operationId: delete-bill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /non_visit_notes/{id}/\n  method: get\n  operationId: get-non-visit-note\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /non_visit_notes/{id}/\n  method: delete\n  operationId: delete-non-visit-note\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /non_visit_notes/{id}/\n  method: put\n  operationId: update-non-visit-note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /non_visit_notes/{id}/\n  method: patch\n  operationId: update-non-visit-note-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /histories/{id}/\n  method: get\n  operationId: get-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /histories/{id}/\n  method: delete\n  operationId: delete-history\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/{id}/\n  method: get\n  operationId: get-report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{id}/\n  method: delete\n  operationId: delete-report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/{id}/\n  method: patch\n  operationId: sign-report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/\n  method: get\n  operationId: find-reports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/\n  method: post\n  operationId: create-report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /vitals/\n  method: get\n  operationId: find-vitals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vitals/\n  method: post\n  operationId: create-vital\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /non_visit_notes/\n  method: get\n  operationId: find-non-visit-notes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /non_visit_notes/\n  method: post\n  operationId: create-non-visit-note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /practices/\n  method: get\n  operationId: find-practices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /family_histories/\n  method: get\n  operationId: find-family-histories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /family_histories/\n  method: post\n  operationId: create-family-history\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /visit_notes/{id}/\n  method: get\n  operationId:\
  \ get-visit-note\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /visit_notes/{id}/\n  method: delete\n  operationId: delete-visit-note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /visit_notes/{id}/\n  method: patch\n  operationId: sign-visit-note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/\n  method: get\n  operationId: find-bills\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bills/\n  method: post\n  operationId: create-bill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /medications/{id}/\n  method: get\n  operationId: get-medication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointments/rooms\n  method: get\n  operationId: find-appointment-rooms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/subscriptions/\n  method: post\n  operationId: subscribe-to-a-resource-updates\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/subscriptions/\n  method: get\n  operationId: find-subscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/published_events/\n  method: get\n  operationId: find-published-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /languages/\n  method: get\n  operationId: find-languages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports-ext/\n  method: post\n  operationId: create-external-report\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recurring_event_groups/{id}/\n  method: get\n  operationId: get-recurring-event-group\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recurring_event_groups/{id}/\n  method: delete\n  operationId: delete-recurring-event-group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointments/id/\n  method: patch\n  operationId: update-appointment-slot\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointments/id/\n  method: put\n  operationId: update-appointment-slot-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointments/slots/\n  method: options\n  operationId: create-appointment-slot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recurring_event_groups/\n  method: post\n  operationId: create-recurring-event-group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recurring_event_groups/\n  method: get\n  operationId: find-recurring-event-group\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recurring_event_groups/:id/\n  method: put\n  operationId: update-recurring-event-group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pharmacies/{ncpdpid}/\n  method: get\n  operationId: get-pharmacy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /broadcast_messages/\n  method: get\n  operationId: find-broadcastmessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broadcast_messages/\n  method: post\n  operationId: create-a-broadcastmessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broadcast_messages/{id}/\n  method: delete\n  operationId: delete-a-broadcastmessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /app/subscriptions/{id}/\n  method: delete\n  operationId: delete-a-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vitals/:id/\n  method: patch\n  operationId: update-vitals-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vitals/:id/\n  method: put\n  operationId: update-vitals\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /insurance_plans/{id}/\n  method: get\n  operationId: get-insurance-plan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insurance_plans/{id}/\n  method: delete\n  operationId: delete-insurance-plan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insurance_companies/\n  method: get\n  operationId: find-insurance-companies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insurance_companies/\n  method: post\n  operationId: create-insurance-company\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insurance_plans/\n  method: get\n  operationId: find-insurance-plans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insurance_plans/\n  method: post\n  operationId: create-insurance-plan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insurance_companies/{id}/\n  method: get\n  operationId: get-insurance-company\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /insurance_companies/{id}/\n  method: delete\n  operationId: delete-insurance-company\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insurance_companies/:id/\n  method: patch\n  operationId: update-insurance-company-2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insurance_companies/:id/\n  method: put\n  operationId: update-insurance-company-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insurance_plans/:id/\n  method: put\n  operationId: update-insurance-plan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insurance_plans/:id/\n  method: patch\n  operationId: update-insurance-plan-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patients/\n  method: post\n  operationId: create-patient\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patients/\n  method: get\n  operationId: find-patients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{id}/printable\n  method: get\n  operationId: retrieve-the-printable-report-view\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ccda/{patient_id}\n  method: get\n  operationId: get-ccda\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/published_events/{event_id}/\n  method: patch\n  operationId: update-published-event-1\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/published_events/{event_id}/\n  method: put\n  operationId: update-published-event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/published_events/{event_id}/\n  method: get\n  operationId: get-published-event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /practices/{id}/\n  method: patch\n  operationId: update-practice-wip-1\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /practices/{id}/\n  method: put\n  operationId: update-practice-wip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /practices/{id}/\n  method: get\n  operationId: get-practice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /physicians/{id}/\n  method: get\n  operationId: get-physician\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /physicians/{id}/\n  method: put\n  operationId: update-physician-wip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /physicians/{id}/\n  method: patch\n  operationId: update-physician-wip-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lab_orders/\n  method: get\n  operationId: find-lab-orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lab_orders/\n  method: post\n  operationId:\
  \ create-lab-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: post\n  operationId: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /message_threads/{id}\n  method: get\n  operationId: get-message-thread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /thread_messages/{id}\n  method: get\n  operationId: get-thread-message\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /thread_message\n\n# --- truncated at 32 KB (249 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/agentic-access/elation-health-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/agentic-access/elation-health-agentic-access.yml
summary_line: 846 operations · 455 acting
tags:
- Healthcare
- United States
- EHR
- EMR
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- Primary Care
- Value-Based Care
- Eligibility
- Clinical Data
- Scheduling
- e-Prescribing
- Digital Health
---

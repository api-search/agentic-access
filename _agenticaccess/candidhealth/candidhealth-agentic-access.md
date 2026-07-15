---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 10
api_specs:
- filename: candidhealth-openapi.yml
  format: yaml
  label: Candid Health Encounters & Claims API
  slug: encounters-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-openapi.yml
- filename: candidhealth-openapi.yml
  format: yaml
  label: Candid Health Eligibility API
  slug: eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-openapi.yml
- filename: candidhealth-openapi.yml
  format: yaml
  label: Candid Health Charge Capture API
  slug: charge-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-openapi.yml
- filename: candidhealth-openapi.yml
  format: yaml
  label: Candid Health Payers & Fee Schedules API
  slug: payers-fee-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-openapi.yml
- filename: candidhealth-openapi.yml
  format: yaml
  label: Candid Health Remits & ERAs API
  slug: remits-eras-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-openapi.yml
- filename: candidhealth-openapi.yml
  format: yaml
  label: Candid Health Webhooks & Events API
  slug: webhooks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/openapi/candidhealth-openapi.yml
consequence_counts:
  physical: 1
  read: 10
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Candidhealth Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charge_captures/v1
operation_count: 15
overview: 'Candid Health exposes 15 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 4 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Candid Health
provider_slug: candidhealth
slug: candidhealth-agentic-access
source_filename: candidhealth-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/candidhealth-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 5\n    connected: 10\n  by_consequence:\n    write: 4\n    read: 10\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/v2/token\n  method: post\n  operationId: getToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encounters/v4\n  method: get\n  operationId: getAllEncounters\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encounters/v4\n  method: post\n  operationId: createEncounter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encounters/v4/{encounter_id}\n  method: get\n  operationId: getEncounter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eligibility/v2\n  method: post\n  operationId: submitEligibilityCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /pre-encounter/coverages/v1/check_eligibility\n  method: post\n  operationId: checkCoverageEligibility\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charge_captures/v1\n  method: post\n  operationId: createChargeCapture\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charge_captures/v1\n  method: get\n  operationId: getAllChargeCaptures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charge_captures/v1/{charge_capture_id}\n  method: get\n  operationId: getChargeCapture\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payers/v3\n  method: get\n  operationId: getAllPayers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payers/v3/{payer_uuid}\n  method: get\n  operationId: getPayer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fee-schedules/v3/service-line/{service_line_id}/match\n  method: get\n  operationId: getFeeScheduleMatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /insurance_adjudications/v1/{insurance_adjudication_id}\n  method: get\n  operationId: getInsuranceAdjudication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/v1\n  method: get\n  operationId: scanEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/v1/{event_id}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/candidhealth/refs/heads/main/agentic-access/candidhealth-agentic-access.yml
summary_line: 15 operations · 5 acting
tags:
- Healthcare
- Medical Billing
- Revenue Cycle
- Claims
- Eligibility
---

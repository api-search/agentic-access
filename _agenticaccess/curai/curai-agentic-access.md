---
acting_count: 2
action_class_counts:
  acting: 2
api_specs:
- filename: curai-partner-openapi.json
  format: json
  label: Curai Partner API
  slug: curai-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curai/refs/heads/main/openapi/curai-partner-openapi.json
consequence_counts:
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Curai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'Curai exposes 2 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Curai
provider_slug: curai
slug: curai-agentic-access
source_filename: curai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/curai-partner-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    acting: 2\n  by_consequence:\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /register-patient\n  method: post\n  operationId: Register_Patient_register_patient_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /end-service\n  method: post\n  operationId: End_Service_end_service_post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curai/refs/heads/main/agentic-access/curai-agentic-access.yml
summary_line: 2 operations · 2 acting
tags:
- Company
- Health
- Healthcare
- Telemedicine
- Telehealth
- Primary Care
- Digital Health
- Patient Engagement
- Partner API
- SDK
---

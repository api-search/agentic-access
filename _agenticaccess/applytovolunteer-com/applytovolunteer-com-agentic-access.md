---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 12
api_specs:
- filename: applytovolunteer-com-applications-api-openapi.yml
  format: yaml
  label: ApplyToVolunteer Applications API
  slug: applytovolunteer-com-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/applytovolunteer-com/openapi/applytovolunteer-com-applications-api-openapi.yml
- filename: applytovolunteer-com-auth-api-openapi.yml
  format: yaml
  label: ApplyToVolunteer Auth API
  slug: applytovolunteer-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/applytovolunteer-com/openapi/applytovolunteer-com-auth-api-openapi.yml
- filename: applytovolunteer-com-conversions-api-openapi.yml
  format: yaml
  label: ApplyToVolunteer Conversions API
  slug: applytovolunteer-com-conversions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/applytovolunteer-com/openapi/applytovolunteer-com-conversions-api-openapi.yml
- filename: applytovolunteer-com-demos-api-openapi.yml
  format: yaml
  label: ApplyToVolunteer Demos API
  slug: applytovolunteer-com-demos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/applytovolunteer-com/openapi/applytovolunteer-com-demos-api-openapi.yml
- filename: applytovolunteer-com-forms-api-openapi.yml
  format: yaml
  label: ApplyToVolunteer Forms API
  slug: applytovolunteer-com-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/applytovolunteer-com/openapi/applytovolunteer-com-forms-api-openapi.yml
- filename: applytovolunteer-com-me-api-openapi.yml
  format: yaml
  label: ApplyToVolunteer Me API
  slug: applytovolunteer-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/applytovolunteer-com/openapi/applytovolunteer-com-me-api-openapi.yml
- filename: applytovolunteer-com-public-api-openapi.yml
  format: yaml
  label: ApplyToVolunteer Public API
  slug: applytovolunteer-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/applytovolunteer-com/openapi/applytovolunteer-com-public-api-openapi.yml
- filename: applytovolunteer-com-tools-api-openapi.yml
  format: yaml
  label: ApplyToVolunteer Tools API
  slug: applytovolunteer-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/applytovolunteer-com/openapi/applytovolunteer-com-tools-api-openapi.yml
consequence_counts:
  physical: 1
  read: 12
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Applytovolunteer Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/auth/magic-link
operation_count: 26
overview: 'ApplyToVolunteer exposes 26 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 13 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ApplyToVolunteer
provider_slug: applytovolunteer-com
slug: applytovolunteer-com-agentic-access
source_filename: applytovolunteer-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/applytovolunteer-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 12\n    acting: 14\n  by_consequence:\n    read: 12\n    physical: 1\n    write: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/me\n  method: get\n  operationId: getCurrentSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auth/magic-link\n  method: post\n  operationId: sendMagicLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/auth/verify\n  method: get\n  operationId: verifyMagicLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auth/verify\n  method: head\n  operationId: probeMagicLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auth/verify\n  method: post\n  operationId: confirmMagicLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/demos/claim/verify\n\
  \  method: head\n  operationId: probeClaimLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/conversions\n  method: post\n  operationId: createConversion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/conversions/{id}\n  method: get\n  operationId: getConversion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/forms\n  method: get\n  operationId: listForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/forms\n\
  \  method: post\n  operationId: createForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/forms/{id}\n  method: get\n  operationId: getForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/forms/{id}\n  method: patch\n  operationId: updateForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/forms/{id}/publish\n  method: post\n  operationId: publishForm\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/forms/{id}/repair-identities\n  method: post\n  operationId: repairFormFieldIdentities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/forms/{id}/discard\n  method: post\n  operationId: discardFormDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/forms/{id}/grade\n\
  \  method: get\n  operationId: gradeSavedForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/forms/{id}/applications\n  method: get\n  operationId: listFormApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/applications/{id}\n  method: get\n  operationId: getApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/applications/{id}\n  method: patch\n  operationId: updateApplicationStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /public/forms/{org}/{form}/submit\n  method: post\n  operationId: submitPublicForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/continue/{token}/submit\n  method: post\n  operationId: submitContinueStage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/grade\n  method: post\n  operationId: gradePublicForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/grade/{id}\n  method: get\n  operationId: getPublicGrade\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/convert\n  method: post\n  operationId: createFormPreview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/previews/{id}\n  method: get\n  operationId: getFormPreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/previews/{id}/claim\n  method: post\n  operationId:\
  \ claimFormPreview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/applytovolunteer-com/agentic-access/applytovolunteer-com-agentic-access.yml
summary_line: 26 operations · 14 acting
tags:
- Volunteer
- Forms
- Software-as-a-Service
- Non-Profit
- Platform
---

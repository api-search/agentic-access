---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 10
api_specs:
- filename: go1-openapi.yml
  format: yaml
  label: Go1 API
  slug: go1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-openapi.yml
consequence_counts:
  read: 10
  safety-critical: 5
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Go1 Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /enrollments
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /enrollments/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /enrollments/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /webhooks
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /webhooks/{id}
operation_count: 20
overview: 'Go1 exposes 20 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 5 write, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Go1
provider_slug: go1
slug: go1-agentic-access
source_filename: go1-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/go1-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 10\n    acting: 10\n  by_consequence:\n    read: 10\n    safety-critical: 5\n    write: 5\n  human_in_the_loop_required: 5\noperations:\n- path: /webhooks\n  method: get\n  operationId: WebhookController_getPortalWebhookConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhook.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: WebhookController_createPortalWebhookConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    scope:\n    - webhook.write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /webhooks/{id}\n  method: patch\n  operationId: WebhookController_updatePortalWebhookConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - webhook.write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /learning-objects/{id}/alternatives\n  method: get\n  operationId: getRetiringContentAlternatives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - lo.read\n    - portal.read\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /learning-objects/{id}\n  method: get\n  operationId: learning-objects-v3-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - lo.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /learning-objects/{id}\n  method: delete\n  operationId: learning-objects-v3-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - lo.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /learning-objects\n  method: get\n  operationId: learning-objects-v3-search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - lo.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /learning-objects\n  method: post\n  operationId: learning-objects-v3-create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - lo.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /learning-objects/{id}/set\n  method: post\n  operationId: learning-objects-v3-update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - lo.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /learning-objects/{id}/scorm\n  method: get\n  operationId: learning-objects-download-scorm-package\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - lo.write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrollments/{id}\n\
  \  method: get\n  operationId: enrolmentLoadController_getSlimEnrollment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - enrollment.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrollments/{id}\n  method: patch\n  operationId: enrolmentLoadController_patchSlimEnrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - enrollment.write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /enrollments/{id}\n  method: delete\n  operationId: enrolmentDeleteController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - enrollment.write\n    audience: null\n    token:\n      max-ttl: 120\n    \
  \  exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /enrollments\n  method: get\n  operationId: enrolmentSearchController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - enrollment.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrollments\n  method: post\n  operationId: enrolmentCreateController_postV3\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - enrollment.write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /enrollments/{id}/certificate\n  method: get\n  operationId: download_enrollment_controller\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - enrollment.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portals\n  method: post\n  operationId: createPortal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - portal.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portals\n  method: get\n  operationId: getPortals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - portal.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portals/{id}\n  method: get\n  operationId: getPortal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - portal.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portals/{id}\n\
  \  method: patch\n  operationId: patchPortal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - portal.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/agentic-access/go1-agentic-access.yml
summary_line: 20 operations · 10 acting · 5 human-in-the-loop
tags:
- Company
- Edtech
- Learning
- E-Learning
- Corporate Training
- Content
- Learning Management
- LMS
- Education
- Webhooks
---

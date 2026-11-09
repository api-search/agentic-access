---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 11
api_specs:
- filename: sendar-app-emails-api-openapi.yml
  format: yaml
  label: sendar-app Emails API
  slug: sendar-app-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendar-app/openapi/sendar-app-emails-api-openapi.yml
- filename: sendar-app-headless-api-openapi.yml
  format: yaml
  label: sendar-app Headless API
  slug: sendar-app-headless-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendar-app/openapi/sendar-app-headless-api-openapi.yml
- filename: sendar-app-inboxes-api-openapi.yml
  format: yaml
  label: sendar-app Inboxes API
  slug: sendar-app-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendar-app/openapi/sendar-app-inboxes-api-openapi.yml
- filename: sendar-app-link-checks-api-openapi.yml
  format: yaml
  label: sendar-app Link Checks API
  slug: sendar-app-link-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendar-app/openapi/sendar-app-link-checks-api-openapi.yml
consequence_counts:
  physical: 4
  read: 11
  safety-critical: 2
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Sendar App Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /inboxes/{inboxId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /link-checks/{id}/override
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /emails
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /emails/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /inboxes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /inboxes/{inboxId}/messages/{messageId}/reply
operation_count: 19
overview: 'sendar-app exposes 19 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 2 write, 4 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: sendar-app
provider_slug: sendar-app
slug: sendar-app-agentic-access
source_filename: sendar-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/sendar-app-headless-openapi.json, openapi/sendar-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 11\n    acting: 8\n  by_consequence:\n    read: 11\n    write: 2\n    safety-critical: 2\n    physical: 4\n  human_in_the_loop_required: 2\noperations:\n- path: /headless/capabilities\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link-checks\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /link-checks/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link-checks/{id}/override\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /inboxes/status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inboxes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /inboxes\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inboxes/{inboxId}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /inboxes/{inboxId}/messages\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inboxes/{inboxId}/messages/{messageId}\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inboxes/{inboxId}/messages/{messageId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inboxes/{inboxId}/messages/{messageId}/raw\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inboxes/{inboxId}/messages/{messageId}/attachments/{index}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inboxes/{inboxId}/messages/{messageId}/reply\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emails\n  method: get\n  operationId: listEmails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emails\n  method: post\n  operationId: sendEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emails/{id}\n  method: get\n  operationId: getEmail\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emails/{id}/events\n  method: get\n  operationId: listEmailEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emails/batch\n  method: post\n  operationId: sendBatchEmails\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/sendar-app/agentic-access/sendar-app-agentic-access.yml
summary_line: 19 operations · 8 acting · 2 human-in-the-loop
tags:
- Company
- Logistics
- Delivery
- Automation
---

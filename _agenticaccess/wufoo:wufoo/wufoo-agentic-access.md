---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 14
api_specs:
- filename: wufoo-rest-v3-openapi.yml
  format: yaml
  label: Wufoo REST API v3
  slug: wufoo:rest-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo:wufoo/refs/heads/main/openapi/wufoo-rest-v3-openapi.yml
- filename: wufoo-webhooks-asyncapi.yml
  format: yaml
  label: Wufoo Webhooks
  slug: wufoo:webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo:wufoo/refs/heads/main/asyncapi/wufoo-webhooks-asyncapi.yml
consequence_counts:
  read: 14
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wufoo Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Wufoo exposes 18 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wufoo
provider_slug: wufoo:wufoo
slug: wufoo-agentic-access
source_filename: wufoo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wufoo-rest-v3-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 14\n    acting: 4\n  by_consequence:\n    read: 14\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /forms.{format}\n  method: get\n  operationId: listForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forms/{identifier}.{format}\n  method: get\n  operationId: getForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forms/{identifier}/fields.{format}\n\
  \  method: get\n  operationId: listFormFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forms/{identifier}/entries.{format}\n  method: get\n  operationId: listFormEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forms/{identifier}/entries.{format}\n  method: post\n  operationId: submitFormEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /forms/{identifier}/entries/count.{format}\n  method: get\n  operationId: countFormEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /forms/{identifier}/comments.{format}\n  method: get\n  operationId: listFormComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forms/{identifier}/comments/count.{format}\n  method: get\n  operationId: countFormComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports.{format}\n  method: get\n  operationId: listReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{identifier}.{format}\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{identifier}/widgets.{format}\n\
  \  method: get\n  operationId: listReportWidgets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{identifier}/entries.{format}\n  method: get\n  operationId: listReportEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{identifier}/entries/count.{format}\n  method: get\n  operationId: countReportEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{identifier}/fields.{format}\n  method: get\n  operationId: listReportFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users.{format}\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{identifier}.{format}\n  method: put\n  operationId: putFormWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{identifier}/{hash}.{format}\n  method: delete\n  operationId: deleteFormWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /login.{format}\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wufoo:wufoo/refs/heads/main/agentic-access/wufoo-agentic-access.yml
summary_line: 18 operations · 4 acting
tags:
- Forms
- Form Builder
- Surveys
- Data Collection
- Webhooks
- Payments
- SurveyMonkey
---

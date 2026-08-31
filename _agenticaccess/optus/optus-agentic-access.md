---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 8
api_specs:
- filename: optus-delete-multiple-lists-api-openapi.yml
  format: yaml
  label: Optus Delete Multiple Lists API
  slug: optus-delete-multiple-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-delete-multiple-lists-api-openapi.yml
- filename: optus-documentation-api-openapi.yml
  format: yaml
  label: Optus Documentation API
  slug: optus-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-documentation-api-openapi.yml
- filename: optus-lists-api-openapi.yml
  format: yaml
  label: Optus Lists API
  slug: optus-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-lists-api-openapi.yml
- filename: optus-messages-api-openapi.yml
  format: yaml
  label: Optus Messages API
  slug: optus-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-messages-api-openapi.yml
- filename: optus-report-api-openapi.yml
  format: yaml
  label: Optus Report API
  slug: optus-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-report-api-openapi.yml
- filename: optus-scheduled-campaigns-api-openapi.yml
  format: yaml
  label: Optus Scheduled Campaigns API
  slug: optus-scheduled-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-scheduled-campaigns-api-openapi.yml
- filename: optus-services-api-openapi.yml
  format: yaml
  label: Optus Services API
  slug: optus-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-services-api-openapi.yml
- filename: optus-status-api-openapi.yml
  format: yaml
  label: Optus Status API
  slug: optus-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-status-api-openapi.yml
- filename: optus-templates-api-openapi.yml
  format: yaml
  label: Optus Templates API
  slug: optus-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-templates-api-openapi.yml
consequence_counts:
  read: 8
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Optus Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Optus exposes 15 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Optus
provider_slug: optus
slug: optus-agentic-access
source_filename: optus-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/optus-sms-suite-campaign-manager-openapi.yml, openapi/optus-sms-suite-rest-v1-openapi.yml,\n  openapi/optus-sms-suite-rest-v2-openapi.yml, openapi/optus-sms-suite-status-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 7\n    connected: 8\n  by_consequence:\n    write: 7\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /{application_name}/delete_multiple_lists\n  method: post\n  operationId: deleteMultList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /{application_name}/lists\n  method: get\n  operationId: getLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{application_name}/lists\n  method: post\n  operationId: createList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{application_name}/lists/{list_id}\n  method: delete\n  operationId: deleteList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /{application_name}/scheduled_campaigns\n  method: post\n  operationId: scheduleCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{application_name}/templates\n  method: get\n  operationId: getTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{application_name}/{campaign_id}/report\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/broadcast\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/{messageid}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.yaml\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/agentic-access/optus-agentic-access.yml
summary_line: 15 operations · 7 acting
tags:
- Telecommunications
- Australia
- Mobile Network Operator
- Messaging
- SMS
- MMS
- Two-Factor Authentication
- Network APIs
- CAMARA
- Open Gateway
- IoT
- 5G
- Broadband
- Satellite
- Enterprise
---

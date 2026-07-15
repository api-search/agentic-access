---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 17
api_specs:
- filename: downloadOAS
  format: yaml
  label: Zoho Creator REST API v2.1
  slug: zoho-creator-rest-api-v21
  spec_type: OpenAPI
  url: https://creator.zoho.com/api/v2/downloadOAS
consequence_counts:
  read: 17
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zoho Creator Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Zoho Creator exposes 27 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zoho Creator
provider_slug: zoho-creator
slug: zoho-creator-agentic-access
source_filename: zoho-creator-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 17\n    acting: 10\n  by_consequence:\n    read: 17\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /creator/v2/meta/{account_owner_name}/{app_link_name}/sections\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoCreator.meta.application.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creator/v2/publish/{account_owner_name}/{app_link_name}/report/{report_link_name}/{record_ID}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creator/v2/meta/{account_owner_name}/{app_link_name}/form/{form_link_name}/fields\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoCreator.meta.form.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creator/v2/meta/{account_owner_name}/{app_link_name}/reports\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoCreator.meta.application.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creator/v2/data/{account_owner_name}/{app_link_name}/report/{report_link_name}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoCreator.report.UPDATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creator/v2/data/{account_owner_name}/{app_link_name}/report/{report_link_name}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoCreator.report.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creator/v2/data/{account_owner_name}/{app_link_name}/report/{report_link_name}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoCreator.report.DELETE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creator/v2/meta/{account_owner_name}/{app_link_name}/pages\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoCreator.meta.application.READ\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /creator/v2/data/{account_owner_name}/{app_link_name}/report/{report_link_name}/{record_ID}/{field_link_name}/download\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoCreator.report.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creator/v2/data/{account_owner_name}/{app_link_name}/report/{report_link_name}/{record_ID}/{subform_link_name}/{field_link_name}/{subform_record_ID}/download\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoCreator.report.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creator/v2/data/{account_owner_name}/{app_link_name}/report/{report_link_name}/{record_ID}/{field_link_name}/upload\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - ZohoCreator.report.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creator/v2/meta/applications\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoCreator.dashboard.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creator/v2/bulk/{account_owner_name}/{app_link_name}/form/{form_link_name}/insert/{job_ID}/result\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoCreator.bulk.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creator/v2/bulk/{account_owner_name}/{app_link_name}/form/{form_link_name}/insert\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoCreator.bulk.CREATE\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creator/v2/data/{account_owner_name}/{app_link_name}/form/{form_link_name}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoCreator.form.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creator/v2/data/{account_owner_name}/{app_link_name}/report/{report_link_name}/{record_ID}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoCreator.report.UPDATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /creator/v2/data/{account_owner_name}/{app_link_name}/report/{report_link_name}/{record_ID}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoCreator.report.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creator/v2/data/{account_owner_name}/{app_link_name}/report/{report_link_name}/{record_ID}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoCreator.report.DELETE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creator/v2/bulk/{account_owner_name}/{app_link_name}/report/{report_link_name}/read\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - ZohoCreator.bulk.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creator/v2/bulk/{account_owner_name}/{app_link_name}/form/{form_link_name}/insert/{job_ID}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoCreator.bulk.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creator/v2/bulk/{account_owner_name}/{app_link_name}/form/{form_link_name}/insert/{job_ID}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoCreator.bulk.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creator/v2/bulk/{account_owner_name}/{app_link_name}/report/{report_link_name}/read/{job_ID}/result\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoCreator.bulk.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creator/v2/publish/{account_owner_name}/{app_link_name}/report/{report_link_name}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creator/v2/bulk/{account_owner_name}/{app_link_name}/report/{report_link_name}/read/{job_ID}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoCreator.bulk.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creator/v2/meta/{account_owner_name}/applications\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoCreator.dashboard.READ\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /creator/v2/meta/{account_owner_name}/{app_link_name}/forms\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoCreator.meta.application.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creator/v2/publish/{account_owner_name}/{app_link_name}/form/{form_link_name}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-creator/refs/heads/main/agentic-access/zoho-creator-agentic-access.yml
summary_line: 27 operations · 10 acting
tags:
- Low-Code
- Application Development
- No-Code
- Forms
- Records
- Workflows
- Database
- CRUD
- Business Applications
---

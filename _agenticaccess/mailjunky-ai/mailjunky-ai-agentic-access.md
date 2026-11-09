---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 6
api_specs:
- filename: mailjunky-ai-analytics-api-openapi.yml
  format: yaml
  label: mailjunky-ai Analytics API
  slug: mailjunky-ai-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailjunky-ai/openapi/mailjunky-ai-analytics-api-openapi.yml
- filename: mailjunky-ai-auth-api-openapi.yml
  format: yaml
  label: mailjunky-ai Auth API
  slug: mailjunky-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailjunky-ai/openapi/mailjunky-ai-auth-api-openapi.yml
- filename: mailjunky-ai-contacts-api-openapi.yml
  format: yaml
  label: mailjunky-ai Contacts API
  slug: mailjunky-ai-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailjunky-ai/openapi/mailjunky-ai-contacts-api-openapi.yml
- filename: mailjunky-ai-emails-api-openapi.yml
  format: yaml
  label: mailjunky-ai Emails API
  slug: mailjunky-ai-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailjunky-ai/openapi/mailjunky-ai-emails-api-openapi.yml
- filename: mailjunky-ai-events-api-openapi.yml
  format: yaml
  label: mailjunky-ai Events API
  slug: mailjunky-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailjunky-ai/openapi/mailjunky-ai-events-api-openapi.yml
- filename: mailjunky-ai-health-api-openapi.yml
  format: yaml
  label: mailjunky-ai Health API
  slug: mailjunky-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailjunky-ai/openapi/mailjunky-ai-health-api-openapi.yml
consequence_counts:
  physical: 2
  read: 6
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mailjunky Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /emails/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /emails/send
operation_count: 13
overview: 'mailjunky-ai exposes 13 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 5 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: mailjunky-ai
provider_slug: mailjunky-ai
slug: mailjunky-ai-agentic-access
source_filename: mailjunky-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/mailjunky-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 6\n    acting: 7\n  by_consequence:\n    read: 6\n    physical: 2\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/validate\n  method: get\n  operationId: validateApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emails/send\n  method:\
  \ post\n  operationId: sendEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emails/batch\n  method: post\n  operationId: sendBatchEmails\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts\n  method:\
  \ post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{id}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{id}\n  method: patch\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{id}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/batch\n  method: post\n  operationId: batchImportContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/track\n  method: post\n  operationId: trackEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/stats\n  method: get\n  operationId: getEventStats\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: get\n  operationId: getEmailStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/mailjunky-ai/agentic-access/mailjunky-ai-agentic-access.yml
summary_line: 13 operations · 7 acting
tags:
- Company
- Email Marketing
- Artificial Intelligence
- Automation
- Analytics
---

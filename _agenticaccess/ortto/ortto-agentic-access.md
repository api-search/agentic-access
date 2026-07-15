---
acting_count: 11
action_class_counts:
  acting: 11
api_specs:
- filename: ortto-openapi.yml
  format: yaml
  label: Ortto People / Contacts API
  slug: people-contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-openapi.yml
- filename: ortto-openapi.yml
  format: yaml
  label: Ortto Custom Activities API
  slug: custom-activities
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-openapi.yml
- filename: ortto-openapi.yml
  format: yaml
  label: Ortto Campaigns API
  slug: campaigns
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-openapi.yml
- filename: ortto-openapi.yml
  format: yaml
  label: Ortto Tags API
  slug: tags
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-openapi.yml
- filename: ortto-openapi.yml
  format: yaml
  label: Ortto Transactional Email API
  slug: transactional-email
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-openapi.yml
- filename: ortto-openapi.yml
  format: yaml
  label: Ortto Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-openapi.yml
consequence_counts:
  physical: 2
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ortto Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transactional/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transactional/send-sms
operation_count: 11
overview: 'Ortto exposes 11 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 write and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ortto
provider_slug: ortto
slug: ortto-agentic-access
source_filename: ortto-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ortto-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 11\n  by_consequence:\n    write: 9\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /person/merge\n  method: post\n  operationId: mergePeople\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /person/get\n  method: post\n  operationId: getPeople\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /person/get-by-ids\n  method: post\n  operationId: getPeopleByIds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /person/delete\n  method: post\n  operationId: deletePeople\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/merge\n  method: post\n  operationId: mergeAccounts\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /activities/create\n  method: post\n  operationId: createActivities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags/get\n  method: post\n  operationId: getTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaign/calendar\n  method: post\n  operationId: getCampaignCalendar\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaign/reports/get\n  method: post\n  operationId: getCampaignReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactional/send\n  method: post\n  operationId: sendTransactionalEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /transactional/send-sms\n  method: post\n  operationId: sendTransactionalSms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/agentic-access/ortto-agentic-access.yml
summary_line: 11 operations · 11 acting
tags:
- Marketing Automation
- CDP
- Customer Data Platform
- Analytics
- Email
---

---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 17
api_specs:
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Constituents API
  slug: bloomerang-constituents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Households API
  slug: bloomerang-households-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Transactions API
  slug: bloomerang-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Interactions API
  slug: bloomerang-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Notes API
  slug: bloomerang-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Relationships API
  slug: bloomerang-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Custom Fields API
  slug: bloomerang-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Lists API
  slug: bloomerang-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Webhooks API
  slug: bloomerang-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
- filename: bloomerang-openapi.yml
  format: yaml
  label: Bloomerang Accounts and Users API
  slug: bloomerang-accounts-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/openapi/bloomerang-openapi.yml
consequence_counts:
  physical: 1
  read: 17
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bloomerang Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /constituents/{id}/relationships
operation_count: 27
overview: 'Bloomerang exposes 27 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 9 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bloomerang
provider_slug: bloomerang
slug: bloomerang-agentic-access
source_filename: bloomerang-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bloomerang-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 17\n    acting: 10\n  by_consequence:\n    read: 17\n    write: 9\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /constituents\n  method: get\n  operationId: listConstituents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /constituents\n  method: post\n  operationId: createConstituent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /constituents/search\n  method: get\n  operationId: searchConstituents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /constituents/{id}\n  method: get\n  operationId: getConstituent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /constituents/{id}\n  method: patch\n  operationId: updateConstituent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /constituents/{id}/timeline\n  method: get\n  operationId: getConstituentTimeline\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /constituents/{id}/relationships\n  method: get\n  operationId: listConstituentRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /constituents/{id}/relationships\n  method: post\n  operationId: createConstituentRelationship\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /households\n  method: post\n  operationId: createHousehold\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /households/{id}\n  method: get\n  operationId: getHousehold\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /households/{id}\n  method: patch\n  operationId: updateHousehold\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: post\n  operationId:\
  \ createTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/{id}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /interactions\n  method: get\n  operationId: listInteractions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /interactions\n  method: post\n  operationId: createInteraction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /interactions/{id}\n  method: get\n  operationId: getInteraction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notes\n  method: post\n  operationId: createNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notes/{id}\n  method: get\n  operationId: getNote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customFields/{type}\n  method: get\n  operationId: listCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId:\
  \ listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funds\n  method: get\n  operationId: listFunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appeals\n  method: get\n  operationId: listAppeals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomerang/refs/heads/main/agentic-access/bloomerang-agentic-access.yml
summary_line: 27 operations · 10 acting
tags:
- Nonprofit
- Donor Management
- CRM
- Fundraising
- Fundraising Software
---

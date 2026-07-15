---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 3
api_specs:
- filename: tithely-openapi.yml
  format: yaml
  label: Tithe.ly Transactions API
  slug: tithely-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/openapi/tithely-openapi.yml
- filename: tithely-openapi.yml
  format: yaml
  label: Tithe.ly Payments & Tokenization API
  slug: tithely-payments-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/openapi/tithely-openapi.yml
- filename: tithely-openapi.yml
  format: yaml
  label: Tithe.ly Organizations API
  slug: tithely-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/openapi/tithely-openapi.yml
- filename: tithely-openapi.yml
  format: yaml
  label: Tithe.ly Payment Categories (Funds) API
  slug: tithely-payment-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/openapi/tithely-openapi.yml
- filename: tithely-openapi.yml
  format: yaml
  label: Tithe.ly Mail API
  slug: tithely-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/openapi/tithely-openapi.yml
- filename: tithely-openapi.yml
  format: yaml
  label: Tithe.ly Accounts API
  slug: tithely-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/openapi/tithely-openapi.yml
consequence_counts:
  physical: 6
  read: 3
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tithely Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charge-once
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mail
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-methods
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment_category
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payment_category/{id}
operation_count: 11
overview: 'Tithe.ly exposes 11 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 2 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tithe.ly
provider_slug: tithely
slug: tithely-agentic-access
source_filename: tithely-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tithely-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 8\n    connected: 3\n  by_consequence:\n    write: 2\n    read: 3\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{id}\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization-owner/{id}\n  method: get\n  operationId: getOrganizationsByOwner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment_category/{id}\n  method: get\n  operationId: getPaymentCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment_category/{id}\n  method: put\n  operationId: updatePaymentCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_category\n\
  \  method: post\n  operationId: createPaymentCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction\n  method: post\n  operationId: createTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mail\n  method: post\n  operationId: sendMail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-methods\n  method: post\n  operationId: createPaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charge\n  method: post\n  operationId: charge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charge-once\n  method: post\n  operationId: chargeOnce\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tithely/refs/heads/main/agentic-access/tithely-agentic-access.yml
summary_line: 11 operations · 8 acting
tags:
- Church Giving
- Donations
- Fundraising
- Payments
- Nonprofit
- ChMS
- Faith
---

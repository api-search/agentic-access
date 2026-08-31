---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 12
api_specs:
- filename: dailypay-accounts-api-openapi.yml
  format: yaml
  label: DailyPay Accounts API
  slug: dailypay-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-accounts-api-openapi.yml
- filename: dailypay-card-tokenization-api-openapi.yml
  format: yaml
  label: DailyPay Card Tokenization API
  slug: dailypay-card-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-card-tokenization-api-openapi.yml
- filename: dailypay-health-api-openapi.yml
  format: yaml
  label: DailyPay Health API
  slug: dailypay-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-health-api-openapi.yml
- filename: dailypay-jobs-api-openapi.yml
  format: yaml
  label: DailyPay Jobs API
  slug: dailypay-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-jobs-api-openapi.yml
- filename: dailypay-organizations-api-openapi.yml
  format: yaml
  label: DailyPay Organizations API
  slug: dailypay-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-organizations-api-openapi.yml
- filename: dailypay-paychecks-api-openapi.yml
  format: yaml
  label: DailyPay Paychecks API
  slug: dailypay-paychecks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-paychecks-api-openapi.yml
- filename: dailypay-people-api-openapi.yml
  format: yaml
  label: DailyPay People API
  slug: dailypay-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-people-api-openapi.yml
- filename: dailypay-transfers-api-openapi.yml
  format: yaml
  label: DailyPay Transfers API
  slug: dailypay-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-transfers-api-openapi.yml
consequence_counts:
  physical: 1
  read: 12
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dailypay Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rest/transfers
operation_count: 18
overview: 'DailyPay exposes 18 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 5 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DailyPay
provider_slug: dailypay
slug: dailypay-agentic-access
source_filename: dailypay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: generated\nsource: openapi/dailypay-rest-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 12\n    acting: 6\n  by_consequence:\n    read: 12\n    write: 5\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /rest/jobs/{job_id}\n  method: get\n  operationId: readJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - client:admin\n    - client:lookup\n    - user:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/jobs/{job_id}\n  method: patch\n  operationId: updateJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - user:read_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - client:admin\n    - client:lookup\n    - user:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/accounts/{account_id}\n  method: get\n  operationId: readAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - client:admin\n    - client:lookup\n    - user:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/accounts/{account_id}\n  method: delete\n  operationId: deleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user:read_write\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - client:admin\n    - client:lookup\n    - user:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/accounts\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user:read_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/transfers/{transfer_id}\n  method: get\n  operationId: readTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - user:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/transfers\n  method: get\n  operationId: listTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/transfers\n  method: post\n  operationId: createTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - user:read_write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/paychecks/{paycheck_id}\n  method: get\n  operationId: readPaycheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user:read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/paychecks\n  method: get\n  operationId: listPaychecks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/organizations/{organization_id}\n  method: get\n  operationId: readOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - client:admin\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/organizations\n  method: get\n  operationId: listOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - client:admin\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/people/{person_id}\n  method: get\n  operationId: readPerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  scope:\n    - client:admin\n    - user:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/people/{person_id}\n  method: patch\n  operationId: updatePerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user:read_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/generic\n  method: post\n  operationId: createGenericCardToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client:admin\n    - user:read\n- path: /rest/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - health:read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/agentic-access/dailypay-agentic-access.yml
summary_line: 18 operations · 6 acting
tags:
- Company
- Payments
- Payroll
- Human Resources
- Earned Wage Access
- On-Demand Pay
- Financial-Services
- Fintech
- Money Transfer
- Benefits
---

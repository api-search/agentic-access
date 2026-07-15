---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 18
api_specs:
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Customers API
  slug: smartmoving-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Opportunities API
  slug: smartmoving-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Leads API
  slug: smartmoving-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Lead Provider API
  slug: smartmoving-lead-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Jobs & Moves API
  slug: smartmoving-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Reference Data API
  slug: smartmoving-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Webhooks API
  slug: smartmoving-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
consequence_counts:
  read: 18
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Smartmoving Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'SmartMoving exposes 24 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SmartMoving
provider_slug: smartmoving
slug: smartmoving-agentic-access
source_filename: smartmoving-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/smartmoving-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 18\n    acting: 6\n  by_consequence:\n    read: 18\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/search\n  method: get\n  operationId: searchCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}\n  method: put\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}/opportunities\n  method: get\n  operationId: listCustomerOpportunities\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/storage-accounts\n  method: get\n  operationId: listCustomerStorageAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{id}\n  method: get\n  operationId: getOpportunity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/quote/{quoteNumber}\n  method: get\n  operationId: getOpportunityByQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{id}/payments\n  method: get\n  operationId: listOpportunityPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{id}/follow-ups\n  method: get\n  operationId: listOpportunityFollowUps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{id}/follow-ups\n  method: post\n  operationId: createOpportunityFollowUp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opportunities/{id}/jobs\n  method: get\n  operationId: listOpportunityJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{id}/jobs\n  method: post\n  operationId: createJob\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{id}\n  method: delete\n  operationId: deleteJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leads\n  method: get\n  operationId: listLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/{id}\n  method: get\n  operationId: getLead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/statuses\n\
  \  method: get\n  operationId: listLeadStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/salesperson/{id}\n  method: get\n  operationId: listLeadsBySalesperson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/from-provider/v2\n  method: post\n  operationId: createLeadFromProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /branches\n  method: get\n  operationId: listBranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /service-types\n  method: get\n  operationId: listServiceTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /referral-sources\n  method: get\n  operationId: listReferralSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/agentic-access/smartmoving-agentic-access.yml
summary_line: 24 operations · 6 acting
tags:
- Moving Software
- CRM
- Field Service
- Moving Company
- Operations
- Lead Management
- Dispatch
---

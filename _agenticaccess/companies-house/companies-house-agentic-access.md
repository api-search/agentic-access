---
acting_count: 0
action_class_counts:
  connected: 28
api_specs:
- filename: companies-house-charges-api-openapi.yml
  format: yaml
  label: Companies House charges API
  slug: companies-house-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/openapi/companies-house-charges-api-openapi.yml
- filename: companies-house-filinghistory-api-openapi.yml
  format: yaml
  label: Companies House filingHistory API
  slug: companies-house-filinghistory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/openapi/companies-house-filinghistory-api-openapi.yml
- filename: companies-house-insolvency-api-openapi.yml
  format: yaml
  label: Companies House insolvency API
  slug: companies-house-insolvency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/openapi/companies-house-insolvency-api-openapi.yml
- filename: companies-house-officerdisqualifications-api-openapi.yml
  format: yaml
  label: Companies House officerDisqualifications API
  slug: companies-house-officerdisqualifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/openapi/companies-house-officerdisqualifications-api-openapi.yml
- filename: companies-house-officers-api-openapi.yml
  format: yaml
  label: Companies House officers API
  slug: companies-house-officers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/openapi/companies-house-officers-api-openapi.yml
- filename: companies-house-personswithsignificantcontrol-api-openapi.yml
  format: yaml
  label: Companies House personsWithSignificantControl API
  slug: companies-house-personswithsignificantcontrol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/openapi/companies-house-personswithsignificantcontrol-api-openapi.yml
- filename: companies-house-registeredofficeaddress-api-openapi.yml
  format: yaml
  label: Companies House registeredOfficeAddress API
  slug: companies-house-registeredofficeaddress-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/openapi/companies-house-registeredofficeaddress-api-openapi.yml
- filename: companies-house-search-api-openapi.yml
  format: yaml
  label: Companies House search API
  slug: companies-house-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/openapi/companies-house-search-api-openapi.yml
consequence_counts:
  read: 28
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Companies House Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'Companies House exposes 28 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Companies House
provider_slug: companies-house
slug: companies-house-agentic-access
source_filename: companies-house-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/companies-house-public-data-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 28\n  by_consequence:\n    read: 28\n  human_in_the_loop_required: 0\noperations:\n- path: /company/{companyNumber}/registered-office-address\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://api.company-information.service.gov.uk/company/{company_number}/registered-office-address.update\n    - https://identity.company-information.service.gov.uk/user/profile.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/companies\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/officers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/disqualified-officers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dissolved-search/companies\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alphabetical-search/companies\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /advanced-search/companies\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_number}/officers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_number}/appointments/{appointment_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_number}/filing-history/{transaction_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_number}/filing-history\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /disqualified-officers/natural/{officer_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /disqualified-officers/corporate/{officer_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_number}/charges\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_number}/charges/{charge_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /company/{company_number}/insolvency\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_number}/persons-with-significant-control\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_number}/persons-with-significant-control/individual/{notification_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_number}/persons-with-significant-control/individual-beneficial-owner/{notification_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_number}/persons-with-significant-control/corporate-entity/{notification_id}\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_number}/persons-with-significant-control/corporate-entity-beneficial-owner/{notification_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_number}/persons-with-significant-control/legal-person/{notification_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_number}/persons-with-significant-control/legal-person-beneficial-owner/{notification_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_number}/persons-with-significant-control-statements\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_number}/persons-with-significant-control-statements/{statement_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_number}/persons-with-significant-control/super-secure/{super_secure_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_number}/persons-with-significant-control/super-secure-beneficial-owner/{super_secure_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/agentic-access/companies-house-agentic-access.yml
summary_line: 28 operations
tags:
- Companies
- UK Government
- Business Registration
- Company Search
- Officers
- Filing History
- Insolvency
- Charges
- Persons of Significant Control
- Open Data
---

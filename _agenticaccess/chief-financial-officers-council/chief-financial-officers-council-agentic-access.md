---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 14
api_specs:
- filename: chief-financial-officers-council-agencies-api-openapi.yml
  format: yaml
  label: Chief Financial Officers Council Agencies API
  slug: chief-financial-officers-council-agencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chief-financial-officers-council/refs/heads/main/openapi/chief-financial-officers-council-agencies-api-openapi.yml
- filename: chief-financial-officers-council-awards-api-openapi.yml
  format: yaml
  label: Chief Financial Officers Council Awards API
  slug: chief-financial-officers-council-awards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chief-financial-officers-council/refs/heads/main/openapi/chief-financial-officers-council-awards-api-openapi.yml
- filename: chief-financial-officers-council-downloads-api-openapi.yml
  format: yaml
  label: Chief Financial Officers Council Downloads API
  slug: chief-financial-officers-council-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chief-financial-officers-council/refs/heads/main/openapi/chief-financial-officers-council-downloads-api-openapi.yml
- filename: chief-financial-officers-council-federal-accounts-api-openapi.yml
  format: yaml
  label: Chief Financial Officers Council Federal Accounts API
  slug: chief-financial-officers-council-federal-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chief-financial-officers-council/refs/heads/main/openapi/chief-financial-officers-council-federal-accounts-api-openapi.yml
- filename: chief-financial-officers-council-recipients-api-openapi.yml
  format: yaml
  label: Chief Financial Officers Council Recipients API
  slug: chief-financial-officers-council-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chief-financial-officers-council/refs/heads/main/openapi/chief-financial-officers-council-recipients-api-openapi.yml
- filename: chief-financial-officers-council-references-api-openapi.yml
  format: yaml
  label: Chief Financial Officers Council References API
  slug: chief-financial-officers-council-references-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chief-financial-officers-council/refs/heads/main/openapi/chief-financial-officers-council-references-api-openapi.yml
- filename: chief-financial-officers-council-search-api-openapi.yml
  format: yaml
  label: Chief Financial Officers Council Search API
  slug: chief-financial-officers-council-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chief-financial-officers-council/refs/heads/main/openapi/chief-financial-officers-council-search-api-openapi.yml
- filename: chief-financial-officers-council-subawards-api-openapi.yml
  format: yaml
  label: Chief Financial Officers Council Subawards API
  slug: chief-financial-officers-council-subawards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chief-financial-officers-council/refs/heads/main/openapi/chief-financial-officers-council-subawards-api-openapi.yml
consequence_counts:
  read: 14
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chief Financial Officers Council Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Chief Financial Officers Council exposes 15 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chief Financial Officers Council
provider_slug: chief-financial-officers-council
slug: chief-financial-officers-council-agentic-access
source_filename: chief-financial-officers-council-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/chief-financial-officers-council-agencies-api-openapi.yml, openapi/chief-financial-officers-council-awards-api-openapi.yml,\n  openapi/chief-financial-officers-council-downloads-api-openapi.yml, openapi/chief-financial-officers-council-federal-accounts-api-openapi.yml,\n  openapi/chief-financial-officers-council-recipients-api-openapi.yml, openapi/chief-financial-officers-council-references-api-openapi.yml,\n  openapi/chief-financial-officers-council-search-api-openapi.yml, openapi/chief-financial-officers-council-subawards-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 14\n    acting: 1\n  by_consequence:\n    read: 14\n    write:\
  \ 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/agency/{TOPTIER_AGENCY_CODE}/\n  method: get\n  operationId: getAgencyOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/agency/{TOPTIER_AGENCY_CODE}/awards/\n  method: get\n  operationId: getAgencyAwards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/agency/{TOPTIER_AGENCY_CODE}/awards/\n  method: get\n  operationId: getAgencyAwards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/awards/{AWARD_ID}/\n  method: get\n  operationId: getAward\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v2/awards/accounts/\n  method: post\n  operationId: listAwardAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/download/awards/\n  method: post\n  operationId: downloadAwards\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/federal_accounts/{ACCOUNT_CODE}/\n  method: get\n  operationId: getFederalAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/recipient/\n  method: post\n  operationId: listRecipients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/recipient/{HASH_VALUE}/\n  method: get\n  operationId: getRecipient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/references/toptier_agencies/\n  method: get\n  operationId: listToptierAgencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/references/naics/{NAICS_CODE}/\n  method: get\n  operationId: getNaics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/search/spending_by_award/\n  method: post\n  operationId: searchSpendingByAward\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /api/v2/search/spending_by_category/{category}/\n  method: post\n  operationId: searchSpendingByCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/search/spending_over_time/\n  method: post\n  operationId: searchSpendingOverTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/subawards/\n  method: post\n  operationId: querySubawards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chief-financial-officers-council/refs/heads/main/agentic-access/chief-financial-officers-council-agentic-access.yml
summary_line: 15 operations · 1 acting
tags:
- Federal Financial Management
- Federal Government
- Finance
- Government
- OMB
- Treasury
---

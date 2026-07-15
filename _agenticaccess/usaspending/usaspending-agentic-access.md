---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 8
api_specs:
- filename: usaspending-openapi.yml
  format: yaml
  label: USAspending Awards Search API
  slug: usaspending-awards-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/openapi/usaspending-openapi.yml
- filename: usaspending-openapi.yml
  format: yaml
  label: USAspending Agency API
  slug: usaspending-agency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/openapi/usaspending-openapi.yml
- filename: usaspending-openapi.yml
  format: yaml
  label: USAspending Recipient API
  slug: usaspending-recipient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/openapi/usaspending-openapi.yml
- filename: usaspending-openapi.yml
  format: yaml
  label: USAspending Federal Account API
  slug: usaspending-federal-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/openapi/usaspending-openapi.yml
- filename: usaspending-openapi.yml
  format: yaml
  label: USAspending Budget Function API
  slug: usaspending-budget-function-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/openapi/usaspending-openapi.yml
- filename: usaspending-openapi.yml
  format: yaml
  label: USAspending Disaster/Emergency Funding (COVID-19) API
  slug: usaspending-disaster-emergency-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/openapi/usaspending-openapi.yml
- filename: usaspending-openapi.yml
  format: yaml
  label: USAspending Bulk Download API
  slug: usaspending-bulk-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/openapi/usaspending-openapi.yml
- filename: usaspending-openapi.yml
  format: yaml
  label: USAspending References & Autocomplete API
  slug: usaspending-references-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/openapi/usaspending-openapi.yml
- filename: usaspending-openapi.yml
  format: yaml
  label: USAspending Subawards API
  slug: usaspending-subawards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/openapi/usaspending-openapi.yml
consequence_counts:
  read: 8
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Usaspending Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'USAspending.gov exposes 14 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: USAspending.gov
provider_slug: usaspending
slug: usaspending-agentic-access
source_filename: usaspending-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/usaspending-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 6\n    connected: 8\n  by_consequence:\n    write: 6\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /search/spending_by_award/\n  method: post\n  operationId: searchSpendingByAward\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agency/{toptier_code}/\n  method: get\n  operationId: getAgencyOverview\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recipient/\n  method: post\n  operationId: listRecipients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /federal_accounts/{account_number}/\n  method: get\n  operationId: getFederalAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /budget_functions/list_budget_functions/\n  method: get\n  operationId: listBudgetFunctions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /budget_functions/list_budget_subfunctions/\n\
  \  method: get\n  operationId: listBudgetSubfunctions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /disaster/overview/\n  method: get\n  operationId: getDisasterOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulk_download/awards/\n  method: post\n  operationId: createBulkAwardDownload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulk_download/status/\n  method: get\n  operationId: getBulkDownloadStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /bulk_download/list_agencies/\n  method: get\n  operationId: listBulkDownloadAgencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /references/toptier_agencies/\n  method: get\n  operationId: listToptierAgencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocomplete/awarding_agency_office/\n  method: post\n  operationId: autocompleteAwardingAgencyOffice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocomplete/recipient/\n  method: post\n  operationId: autocompleteRecipient\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subawards/\n  method: post\n  operationId: listSubawards\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/agentic-access/usaspending-agentic-access.yml
summary_line: 14 operations · 6 acting
tags:
- Government
- Federal Spending
- Open Data
- Contracts
- Grants
- DATA Act
- Transparency
- Public Sector
---

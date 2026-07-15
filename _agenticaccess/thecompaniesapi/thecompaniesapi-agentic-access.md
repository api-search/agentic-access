---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 29
api_specs:
- filename: thecompaniesapi-openapi.yml
  format: yaml
  label: The Companies API Company Search API
  slug: thecompaniesapi-company-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-openapi.yml
- filename: thecompaniesapi-openapi.yml
  format: yaml
  label: The Companies API Company Enrichment API
  slug: thecompaniesapi-company-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-openapi.yml
- filename: thecompaniesapi-openapi.yml
  format: yaml
  label: The Companies API Company Analytics API
  slug: thecompaniesapi-company-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-openapi.yml
- filename: thecompaniesapi-openapi.yml
  format: yaml
  label: The Companies API Industries API
  slug: thecompaniesapi-industries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-openapi.yml
- filename: thecompaniesapi-openapi.yml
  format: yaml
  label: The Companies API Technologies API
  slug: thecompaniesapi-technologies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-openapi.yml
- filename: thecompaniesapi-openapi.yml
  format: yaml
  label: The Companies API Locations API
  slug: thecompaniesapi-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-openapi.yml
- filename: thecompaniesapi-openapi.yml
  format: yaml
  label: The Companies API Lists API
  slug: thecompaniesapi-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-openapi.yml
- filename: thecompaniesapi-openapi.yml
  format: yaml
  label: The Companies API Actions API
  slug: thecompaniesapi-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-openapi.yml
- filename: thecompaniesapi-openapi.yml
  format: yaml
  label: The Companies API Job Titles Enrichment API
  slug: thecompaniesapi-job-titles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-openapi.yml
consequence_counts:
  read: 29
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Thecompaniesapi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 44
overview: 'The Companies API exposes 44 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: The Companies API
provider_slug: thecompaniesapi
slug: thecompaniesapi-agentic-access
source_filename: thecompaniesapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/thecompaniesapi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 44\n  by_action_class:\n    connected: 29\n    acting: 15\n  by_consequence:\n    read: 29\n    write: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: fetchApiHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/openapi\n  method: get\n  operationId: fetchOpenApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/actions\n  method: get\n  operationId:\
  \ fetchActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/actions\n  method: post\n  operationId: requestAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/actions/{actionId}/retry\n  method: post\n  operationId: retryAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies\n  method: get\n  operationId: searchCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies\n  method: post\n  operationId: searchCompaniesPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{domain}\n  method: get\n  operationId: fetchCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/by-name\n  method: get\n  operationId: searchCompaniesByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/by-prompt\n  method: get\n  operationId: searchCompaniesByPrompt\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/similar\n  method: get\n  operationId: searchSimilarCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/count\n  method: get\n  operationId: countCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/count\n  method: post\n  operationId: countCompaniesPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/by-email\n  method: get\n  operationId: fetchCompanyByEmail\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/by-social\n  method: get\n  operationId: fetchCompanyBySocial\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{domain}/email-patterns\n  method: get\n  operationId: fetchCompanyEmailPatterns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{domain}/ask\n  method: post\n  operationId: askCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{domain}/context\n\
  \  method: get\n  operationId: fetchCompanyContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/analytics\n  method: get\n  operationId: fetchCompaniesAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/analytics/export\n  method: post\n  operationId: exportCompaniesAnalytics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/industries\n  method: get\n  operationId: searchIndustries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/industries/similar\n  method: get\n  operationId: searchIndustriesSimilar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/technologies\n  method: get\n  operationId: searchTechnologies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/locations/cities\n  method: get\n  operationId: searchCities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/locations/counties\n  method: get\n  operationId: searchCounties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/locations/countries\n  method: get\n  operationId: searchCountries\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/locations/states\n  method: get\n  operationId: searchStates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/locations/continents\n  method: get\n  operationId: searchContinents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/job-titles/enrich\n  method: get\n  operationId: enrichJobTitles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/lists\n  method: get\n  operationId: fetchLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/lists\n  method: post\n  operationId: createList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/lists/{listId}\n  method: patch\n  operationId: updateList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/lists/{listId}\n  method: delete\n  operationId: deleteList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v2/lists/{listId}/companies\n  method: get\n  operationId: fetchCompaniesInList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/lists/{listId}/companies\n  method: post\n  operationId: fetchCompaniesInListPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/lists/{listId}/companies/{domain}\n  method: get\n  operationId: fetchCompanyInList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/lists/{listId}/companies/toggle\n  method: patch\n  operationId: toggleCompaniesInList\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/teams/{teamId}\n  method: get\n  operationId: fetchTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/teams/{teamId}\n  method: patch\n  operationId: updateTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/user\n  method: get\n  operationId: fetchUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/prompts\n  method: get\n  operationId: fetchPrompts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/prompts/{promptId}\n  method: delete\n  operationId: deletePrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/prompts/product\n  method: post\n  operationId: productPrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/prompts/segmentation\n\
  \  method: post\n  operationId: promptToSegmentation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/agentic-access/thecompaniesapi-agentic-access.yml
summary_line: 44 operations · 15 acting
tags:
- Company Data
- Data Enrichment
- Firmographics
- Web Intelligence
- B2B Data
- Reference Data
- Company Search
---

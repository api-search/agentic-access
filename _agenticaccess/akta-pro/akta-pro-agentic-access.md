---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 11
api_specs:
- filename: akta-pro-company-api-openapi.yml
  format: yaml
  label: akta.pro Company API
  slug: akta-pro-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akta-pro/refs/heads/main/openapi/akta-pro-company-api-openapi.yml
- filename: akta-pro-list-generation-api-openapi.yml
  format: yaml
  label: akta.pro List Generation API
  slug: akta-pro-list-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akta-pro/refs/heads/main/openapi/akta-pro-list-generation-api-openapi.yml
- filename: akta-pro-news-api-openapi.yml
  format: yaml
  label: akta.pro News API
  slug: akta-pro-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akta-pro/refs/heads/main/openapi/akta-pro-news-api-openapi.yml
- filename: akta-pro-reviews-api-openapi.yml
  format: yaml
  label: akta.pro Reviews API
  slug: akta-pro-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akta-pro/refs/heads/main/openapi/akta-pro-reviews-api-openapi.yml
- filename: akta-pro-supporting-apis-api-openapi.yml
  format: yaml
  label: akta.pro Supporting APIs API
  slug: akta-pro-supporting-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akta-pro/refs/heads/main/openapi/akta-pro-supporting-apis-api-openapi.yml
consequence_counts:
  read: 11
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Akta Pro Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'akta.pro exposes 14 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: akta.pro
provider_slug: akta-pro
slug: akta-pro-agentic-access
source_filename: akta-pro-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: generated\nsource: openapi/akta-pro-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 11\n    acting: 3\n  by_consequence:\n    read: 11\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/news\n  method: get\n  operationId: getNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/search\n  method: get\n  operationId: companySearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/enrichment\n  method: get\n \
  \ operationId: companyEnrichment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/product-reviews\n  method: get\n  operationId: getProductReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/employee-reviews\n  method: get\n  operationId: getEmployeeReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/industry/search\n  method: get\n  operationId: industrySearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/headcount-trends\n  method: get\n  operationId: getHeadcountTrends\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/jobs\n  method: get\n  operationId: getJobPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/posts\n  method: get\n  operationId: getSocialPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/website-traffic\n  method: get\n  operationId: getWebsiteTraffic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/addition-requests\n  method: post\n  operationId: createCompanyAdditionRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/status/{request_id}\n  method: get\n  operationId: getRequestStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/list/generate/companies/\n  method: post\n  operationId: generateCompanyList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/list/filter-builder/\n  method: post\n  operationId: translateQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akta-pro/refs/heads/main/agentic-access/akta-pro-agentic-access.yml
summary_line: 14 operations · 3 acting
tags:
- Company
- Company Data
- Company Intelligence
- News
- Alternative Data
- Private Companies
- Firmographics
- Data Enrichment
- Signals
- MCP
- Market Intelligence
---

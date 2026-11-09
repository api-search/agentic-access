---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 13
api_specs:
- filename: blitz-api-ai-account-api-openapi.yml
  format: yaml
  label: blitz-api-ai Account API
  slug: blitz-api-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blitz-api-ai/openapi/blitz-api-ai-account-api-openapi.yml
- filename: blitz-api-ai-changelog-api-openapi.yml
  format: yaml
  label: blitz-api-ai Changelog API
  slug: blitz-api-ai-changelog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blitz-api-ai/openapi/blitz-api-ai-changelog-api-openapi.yml
- filename: blitz-api-ai-company-api-openapi.yml
  format: yaml
  label: blitz-api-ai Company API
  slug: blitz-api-ai-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blitz-api-ai/openapi/blitz-api-ai-company-api-openapi.yml
- filename: blitz-api-ai-company-enrichment-api-openapi.yml
  format: yaml
  label: blitz-api-ai Company Enrichment API
  slug: blitz-api-ai-company-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blitz-api-ai/openapi/blitz-api-ai-company-enrichment-api-openapi.yml
- filename: blitz-api-ai-company-search-api-openapi.yml
  format: yaml
  label: blitz-api-ai Company Search API
  slug: blitz-api-ai-company-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blitz-api-ai/openapi/blitz-api-ai-company-search-api-openapi.yml
- filename: blitz-api-ai-enrichment-api-openapi.yml
  format: yaml
  label: blitz-api-ai Enrichment API
  slug: blitz-api-ai-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blitz-api-ai/openapi/blitz-api-ai-enrichment-api-openapi.yml
- filename: blitz-api-ai-job-search-api-openapi.yml
  format: yaml
  label: blitz-api-ai Job Search API
  slug: blitz-api-ai-job-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blitz-api-ai/openapi/blitz-api-ai-job-search-api-openapi.yml
- filename: blitz-api-ai-jobs-api-openapi.yml
  format: yaml
  label: blitz-api-ai Jobs API
  slug: blitz-api-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blitz-api-ai/openapi/blitz-api-ai-jobs-api-openapi.yml
- filename: blitz-api-ai-people-enrichment-api-openapi.yml
  format: yaml
  label: blitz-api-ai People Enrichment API
  slug: blitz-api-ai-people-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blitz-api-ai/openapi/blitz-api-ai-people-enrichment-api-openapi.yml
- filename: blitz-api-ai-people-search-api-openapi.yml
  format: yaml
  label: blitz-api-ai People Search API
  slug: blitz-api-ai-people-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blitz-api-ai/openapi/blitz-api-ai-people-search-api-openapi.yml
- filename: blitz-api-ai-search-api-openapi.yml
  format: yaml
  label: blitz-api-ai Search API
  slug: blitz-api-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blitz-api-ai/openapi/blitz-api-ai-search-api-openapi.yml
- filename: blitz-api-ai-utilities-api-openapi.yml
  format: yaml
  label: blitz-api-ai Utilities API
  slug: blitz-api-ai-utilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blitz-api-ai/openapi/blitz-api-ai-utilities-api-openapi.yml
- filename: blitz-api-ai-zeroclick-api-openapi.yml
  format: yaml
  label: blitz-api-ai Zeroclick API
  slug: blitz-api-ai-zeroclick-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blitz-api-ai/openapi/blitz-api-ai-zeroclick-api-openapi.yml
consequence_counts:
  physical: 1
  read: 13
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Blitz Api Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /zeroclick/agent/quote
operation_count: 40
overview: 'blitz-api-ai exposes 40 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 26 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: blitz-api-ai
provider_slug: blitz-api-ai
slug: blitz-api-ai-agentic-access
source_filename: blitz-api-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/agents-openapi.json, openapi/api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    acting: 27\n    connected: 13\n  by_consequence:\n    write: 26\n    read: 13\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/company/tam-by-jobs\n  method: post\n  operationId: postV2CompanyTamByJobs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/company/tam-by-people\n  method: post\n  operationId:\
  \ postV2CompanyTamByPeople\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrichment/company\n  method: post\n  operationId: enrichCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrichment/company-distribution-by-country\n  method: post\n  operationId: companyDistributionByCountry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrichment/company-distribution-by-department\n  method: post\n  operationId: companyDistributionByDepartment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrichment/domain-to-linkedin\n  method: post\n  operationId: domainToLinkedin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrichment/email\n  method: post\n  operationId: enrichEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v2/enrichment/email-to-person\n  method: post\n  operationId: emailToPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrichment/linkedin-to-domain\n  method: post\n  operationId: linkedinToDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrichment/person\n  method: post\n  operationId: postV2EnrichmentPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrichment/phone\n  method: post\n  operationId: enrichPhone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/enrichment/phone-to-person\n  method: post\n  operationId: reversePhoneLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/jobs/company\n  method: post\n  operationId: postV2JobsCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/jobs/search\n  method: post\n  operationId: postV2JobsSearch\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/search/companies\n  method: post\n  operationId: postV2SearchCompanies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/search/employee-finder\n  method: post\n  operationId: employeeFinder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/search/people\n  method: post\n  operationId: postV2SearchPeople\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/search/waterfall-icp-keyword\n  method: post\n  operationId: waterfallIcpSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /zeroclick/agent/quote\n  method: post\n  operationId: sellerAgentQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /changelog/\n  method: get\n  operationId: getChangelog\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/key-info\n  method: get\n  operationId: getV2AccountKey-info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/utils/current-date\n  method: post\n  operationId: postV2UtilsCurrent-date\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/search/employee-finder\n  method: post\n  operationId: postV2SearchEmployee-finder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/search/waterfall-icp-keyword\n  method: post\n  operationId: postV2SearchWaterfall-icp-keyword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/search/companies\n  method: post\n  operationId: postV2SearchCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/search/people\n  method: post\n  operationId: postV2SearchPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/jobs/search\n  method: post\n  operationId: postV2JobsSearch\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/jobs/company\n  method: post\n  operationId: postV2JobsCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/company/tam-by-jobs\n  method: post\n  operationId: postV2CompanyTam-by-jobs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/company/tam-by-people\n  method: post\n  operationId: postV2CompanyTam-by-people\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrichment/person\n  method: post\n  operationId: postV2EnrichmentPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrichment/email\n  method: post\n  operationId: postV2EnrichmentEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/enrichment/phone\n  method: post\n  operationId: postV2EnrichmentPhone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/enrichment/email-to-person\n  method: post\n  operationId: postV2EnrichmentEmail-to-person\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrichment/phone-to-person\n  method: post\n  operationId: postV2EnrichmentPhone-to-person\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrichment/domain-to-linkedin\n  method: post\n  operationId: postV2EnrichmentDomain-to-linkedin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/enrichment/linkedin-to-domain\n  method: post\n  operationId: postV2EnrichmentLinkedin-to-domain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrichment/company\n  method: post\n  operationId: postV2EnrichmentCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrichment/company-distribution-by-country\n  method: post\n  operationId: postV2EnrichmentCompany-distribution-by-country\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrichment/company-distribution-by-department\n  method: post\n  operationId: postV2EnrichmentCompany-distribution-by-department\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/blitz-api-ai/agentic-access/blitz-api-ai-agentic-access.yml
summary_line: 40 operations · 27 acting
tags:
- B2B
- Data
- Data Enrichment
- Go-To-Market
---

---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 31
api_specs:
- filename: peopledatalabs-autocomplete-api-openapi.yml
  format: yaml
  label: People Data Labs Autocomplete API
  slug: peopledatalabs-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-autocomplete-api-openapi.yml
- filename: peopledatalabs-cleaner-endpoints-api-openapi.yml
  format: yaml
  label: People Data Labs Cleaner Endpoints API
  slug: peopledatalabs-cleaner-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-cleaner-endpoints-api-openapi.yml
- filename: peopledatalabs-company-endpoints-api-openapi.yml
  format: yaml
  label: People Data Labs Company Endpoints API
  slug: peopledatalabs-company-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-company-endpoints-api-openapi.yml
- filename: peopledatalabs-ip-enrichment-api-openapi.yml
  format: yaml
  label: People Data Labs IP Enrichment API
  slug: peopledatalabs-ip-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-ip-enrichment-api-openapi.yml
- filename: peopledatalabs-job-title-enrichment-api-openapi.yml
  format: yaml
  label: People Data Labs Job Title Enrichment API
  slug: peopledatalabs-job-title-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-job-title-enrichment-api-openapi.yml
- filename: peopledatalabs-person-endpoints-api-openapi.yml
  format: yaml
  label: People Data Labs Person Endpoints API
  slug: peopledatalabs-person-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-person-endpoints-api-openapi.yml
- filename: peopledatalabs-skill-enrichment-api-openapi.yml
  format: yaml
  label: People Data Labs Skill Enrichment API
  slug: peopledatalabs-skill-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-skill-enrichment-api-openapi.yml
- filename: peopledatalabs-subscription-api-openapi.yml
  format: yaml
  label: People Data Labs Subscription API
  slug: peopledatalabs-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-subscription-api-openapi.yml
- filename: peopledatalabs-company-api-openapi.yml
  format: yaml
  label: People Data Labs Company API
  slug: peopledatalabs-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-company-api-openapi.yml
- filename: peopledatalabs-ip-api-openapi.yml
  format: yaml
  label: People Data Labs IP API
  slug: peopledatalabs-ip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-ip-api-openapi.yml
- filename: peopledatalabs-jobs-api-openapi.yml
  format: yaml
  label: People Data Labs Jobs API
  slug: peopledatalabs-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-jobs-api-openapi.yml
- filename: peopledatalabs-person-api-openapi.yml
  format: yaml
  label: People Data Labs Person API
  slug: peopledatalabs-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-person-api-openapi.yml
- filename: peopledatalabs-job-title-api-openapi.yml
  format: yaml
  label: People Data Labs Job Title API
  slug: peopledatalabs-job-title-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-job-title-api-openapi.yml
consequence_counts:
  read: 31
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Peopledatalabs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 46
overview: 'People Data Labs exposes 46 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: People Data Labs
provider_slug: peopledatalabs
slug: peopledatalabs-agentic-access
source_filename: peopledatalabs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/peopledatalabs-autocomplete-api-openapi.yml, openapi/peopledatalabs-cleaner-endpoints-api-openapi.yml,\n  openapi/peopledatalabs-company-api-openapi.yml, openapi/peopledatalabs-company-endpoints-api-openapi.yml,\n  openapi/peopledatalabs-ip-api-openapi.yml, openapi/peopledatalabs-ip-enrichment-api-openapi.yml,\n  openapi/peopledatalabs-job-title-api-openapi.yml, openapi/peopledatalabs-job-title-enrichment-api-openapi.yml,\n  openapi/peopledatalabs-jobs-api-openapi.yml, openapi/peopledatalabs-person-api-openapi.yml,\n  openapi/peopledatalabs-person-endpoints-api-openapi.yml, openapi/peopledatalabs-skill-enrichment-api-openapi.yml,\n  openapi/peopledatalabs-subscription-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\n\
  summary:\n  operations: 46\n  by_action_class:\n    connected: 31\n    acting: 15\n  by_consequence:\n    read: 31\n    write: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /v5/autocomplete\n  method: get\n  operationId: getV5Autocomplete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/autocomplete\n  method: post\n  operationId: postV5Autocomplete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/company/clean\n  method: get\n  operationId: getV5CompanyClean\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/company/clean\n\
  \  method: post\n  operationId: postV5CompanyClean\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/school/clean\n  method: get\n  operationId: getV5SchoolClean\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/school/clean\n  method: post\n  operationId: postV5SchoolClean\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/location/clean\n  method: get\n  operationId: getV5LocationClean\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/location/clean\n  method: post\n  operationId: postV5LocationClean\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/company/enrich\n  method: get\n  operationId: getV5CompanyEnrich\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/company/search\n  method: get\n  operationId: getV5CompanySearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/company/search\n  method: post\n  operationId: postV5CompanySearch\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /company/enrich\n  method: get\n  operationId: getCompanyEnrich\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/search\n  method: get\n  operationId: getCompanySearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/company/enrich\n  method: get\n  operationId: getV5CompanyEnrich\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/company/search\n  method: get\n  operationId: getV5CompanySearch\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/company/search\n  method: post\n  operationId: postV5CompanySearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ip/enrich\n  method: get\n  operationId: getIpEnrich\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/ip/enrich\n  method: get\n  operationId: getV5IpEnrich\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/job_title/enrich\n  method: get\n  operationId: getV5JobTitleEnrich\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/job_title/enrich\n  method: get\n  operationId: getV5JobTitleEnrich\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/job_title/enrich\n  method: post\n  operationId: postV5JobTitleEnrich\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job_posting/search\n  method: get\n  operationId: getJobPostingSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/person/subjectrequest\n  method:\
  \ get\n  operationId: getV5PersonSubjectrequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/person/enrich\n  method: get\n  operationId: getV5PersonEnrich\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/person/enrich/preview\n  method: get\n  operationId: getV5PersonEnrichPreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/person/identify\n  method: get\n  operationId: getV5PersonIdentify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/person/search\n  method: get\n  operationId: getV5PersonSearch\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/person/search\n  method: post\n  operationId: postV5PersonSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/person/retrieve/{person_id}\n  method: get\n  operationId: getV5PersonRetrieveByPersonId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/person/retrieve/bulk\n  method: post\n  operationId: postV5PersonRetrieveBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /person/enrich\n  method: get\n  operationId: getPersonEnrich\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /person/search\n  method: get\n  operationId: getPersonSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /person/identify\n  method: get\n  operationId: getPersonIdentify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /person/bulk\n  method: post\n  operationId: postPersonBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v5/person/enrich\n  method: get\n  operationId: getV5PersonEnrich\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/person/identify\n  method: get\n  operationId: getV5PersonIdentify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/person/search\n  method: get\n  operationId: getV5PersonSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/person/search\n  method: post\n  operationId: postV5PersonSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/person/retrieve/{person_id}\n  method: get\n  operationId: getV5PersonRetrieveByPersonId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/person/retrieve/bulk\n  method: post\n  operationId: postV5PersonRetrieveBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/skill/enrich\n  method: get\n  operationId: getV5SkillEnrich\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/subscription/{subscription_id}\n  method: get\n  operationId: getV5SubscriptionBySubscriptionId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/subscription/{subscription_id}\n  method: delete\n  operationId: deleteV5SubscriptionBySubscriptionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/subscription/{subscription_id}\n  method: put\n  operationId: putV5SubscriptionBySubscriptionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/subscription\n  method: get\n  operationId: getV5Subscription\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/subscription\n  method: post\n  operationId: postV5Subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/agentic-access/peopledatalabs-agentic-access.yml
summary_line: 46 operations · 15 acting
tags:
- Data Enrichment
- Web Intelligence
- Person Data
- Company Data
- B2B Data
- Contact Discovery
- Reference Data
- Firmographics
- Identity Resolution
---

---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 22
api_specs:
- filename: jobspipe-account-api-openapi.yml
  format: yaml
  label: JobsPipe Account API
  slug: jobspipe-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-account-api-openapi.yml
- filename: jobspipe-billing-api-openapi.yml
  format: yaml
  label: JobsPipe Billing API
  slug: jobspipe-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-billing-api-openapi.yml
- filename: jobspipe-companies-api-openapi.yml
  format: yaml
  label: JobsPipe Companies API
  slug: jobspipe-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-companies-api-openapi.yml
- filename: jobspipe-jobs-api-openapi.yml
  format: yaml
  label: JobsPipe Jobs API
  slug: jobspipe-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-jobs-api-openapi.yml
- filename: jobspipe-jobspipe-api-api-openapi.yml
  format: yaml
  label: JobsPipe JobsPipe API
  slug: jobspipe-jobspipe-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-jobspipe-api-api-openapi.yml
- filename: jobspipe-labour-market-insights-api-openapi.yml
  format: yaml
  label: JobsPipe Labour Market Insights API
  slug: jobspipe-labour-market-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-labour-market-insights-api-openapi.yml
- filename: jobspipe-monitors-api-openapi.yml
  format: yaml
  label: JobsPipe Monitors API
  slug: jobspipe-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-monitors-api-openapi.yml
- filename: jobspipe-sandbox-api-openapi.yml
  format: yaml
  label: JobsPipe Sandbox API
  slug: jobspipe-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-sandbox-api-openapi.yml
- filename: jobspipe-stack-api-openapi.yml
  format: yaml
  label: JobsPipe Stack API
  slug: jobspipe-stack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-stack-api-openapi.yml
- filename: jobspipe-technologies-api-openapi.yml
  format: yaml
  label: JobsPipe Technologies API
  slug: jobspipe-technologies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-technologies-api-openapi.yml
consequence_counts:
  physical: 1
  read: 22
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Jobspipe Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/checkout
operation_count: 33
overview: 'JobsPipe exposes 33 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 10 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: JobsPipe
provider_slug: jobspipe
slug: jobspipe-agentic-access
source_filename: jobspipe-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: generated\nsource: openapi/jobspipe-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 22\n    acting: 11\n  by_consequence:\n    read: 22\n    write: 10\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/jobs/search\n  method: post\n  operationId: searchJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/agentic-search\n  method: post\n  operationId: agenticSearchJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stack/scan\n  method: post\n  operationId: scanStack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - stack:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{key}\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/search\n  method: post\n  operationId: searchCompaniesByTechnology\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{key}/technologies\n  method: get\n  operationId:\
  \ getCompanyTechnologies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/technologies\n  method: get\n  operationId: listTechnologies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/technologies/export\n  method: get\n  operationId: exportTechnologies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/technologies/{slug}\n  method: get\n  operationId: getTechnology\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors\n  method: post\n\
  \  operationId: createMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - jobs:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors\n  method: get\n  operationId: listMonitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors/{id}\n  method: get\n  operationId: getMonitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors/{id}\n  method: delete\n  operationId: deleteMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - jobs:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors/{id}/renew\n  method: post\n  operationId: renewMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - jobs:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors/{id}/ids\n  method: post\n  operationId: addMonitorIds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - jobs:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors/{id}/ids\n\
  \  method: delete\n  operationId: removeMonitorIds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - jobs:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors/{id}/ids\n  method: get\n  operationId: listMonitorIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - jobs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/checkout\n  method: post\n  operationId: createBillingCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    scope:\n    - jobs:read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/insights/occupations\n  method: get\n  operationId: insightsOccupations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/insights/occupations/{code}\n  method: get\n  operationId: insightsOccupationSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/insights/occupations/{code}/compensation\n  method: get\n  operationId: insightsCompensation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/insights/occupations/{code}/skills/top\n  method: get\n  operationId: insightsTopSkills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/insights/occupations/{code}/skills/trending\n  method: get\n  operationId: insightsTrendingSkillsByOccupation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/insights/industries\n  method: get\n  operationId: insightsIndustries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/insights/industries/{division}/skills/trending\n  method: get\n  operationId: insightsTrendingSkillsByIndustry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /v1/insights/skills/{slug}/trend\n  method: get\n  operationId: insightsSkillTrend\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/insights/technology/ai-exposure\n  method: get\n  operationId: insightsAiExposure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/insights/salary/benchmark\n  method: post\n  operationId: insightsSalaryBenchmark\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sandbox/jobs/search\n  method: post\n  operationId: sandboxSearchJobs\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sandbox/jobs/search/batch\n  method: post\n  operationId: sandboxSearchJobsBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sandbox/jobs/export\n  method: post\n  operationId: sandboxCreateExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sandbox/jobs/export/{id}\n\
  \  method: get\n  operationId: sandboxGetExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/agentic-access/jobspipe-agentic-access.yml
summary_line: 33 operations · 11 acting
tags:
- Company
- Jobs
- API
- Data
- Hiring
---

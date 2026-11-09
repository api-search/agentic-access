---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 11
api_specs:
- filename: veritahire-com-account-api-openapi.yml
  format: yaml
  label: veritahire-com Account API
  slug: veritahire-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veritahire-com/openapi/veritahire-com-account-api-openapi.yml
- filename: veritahire-com-employer-profile-api-openapi.yml
  format: yaml
  label: veritahire-com Employer profile API
  slug: veritahire-com-employer-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veritahire-com/openapi/veritahire-com-employer-profile-api-openapi.yml
- filename: veritahire-com-free-no-key-api-openapi.yml
  format: yaml
  label: veritahire-com Free, no key API
  slug: veritahire-com-free-no-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veritahire-com/openapi/veritahire-com-free-no-key-api-openapi.yml
- filename: veritahire-com-hiring-market-php-api-openapi.yml
  format: yaml
  label: veritahire-com Hiring Market.php API
  slug: veritahire-com-hiring-market-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veritahire-com/openapi/veritahire-com-hiring-market-php-api-openapi.yml
- filename: veritahire-com-hiring-velocity-api-openapi.yml
  format: yaml
  label: veritahire-com Hiring velocity API
  slug: veritahire-com-hiring-velocity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veritahire-com/openapi/veritahire-com-hiring-velocity-api-openapi.yml
- filename: veritahire-com-postings-api-openapi.yml
  format: yaml
  label: veritahire-com Postings API
  slug: veritahire-com-postings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veritahire-com/openapi/veritahire-com-postings-api-openapi.yml
consequence_counts:
  read: 11
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Veritahire Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'veritahire-com exposes 13 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: veritahire-com
provider_slug: veritahire-com
slug: veritahire-com-agentic-access
source_filename: veritahire-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/veritahire-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 11\n    acting: 2\n  by_consequence:\n    read: 11\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/benchmark.php\n  method: get\n  operationId: benchmarkRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/job-status.php\n  method: get\n  operationId: isJobStillOpen\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/benchmark-claim.php\n\
  \  method: post\n  operationId: requestFullReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/jobs-search.php\n  method: get\n  operationId: searchLiveJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/job.php\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/jobs-save.php\n  method: post\n  operationId: saveSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/jobs.php\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/velocity.php\n  method: get\n  operationId: velocity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/employers.php\n  method: get\n  operationId: employers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/hiring-market.php\n  method: get\n  operationId: hiringMarket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/hiring-signals.php\n  method:\
  \ get\n  operationId: hiringSignals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/job-openings-index.php\n  method: get\n  operationId: jobOpeningsIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/balance.php\n  method: get\n  operationId: balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/veritahire-com/agentic-access/veritahire-com-agentic-access.yml
summary_line: 13 operations · 2 acting
tags:
- Company
- Job
- Hiring
- Data
---

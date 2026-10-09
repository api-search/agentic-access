---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 7
api_specs:
- filename: mrscraper-analytic-api-openapi.yml
  format: yaml
  label: MrScraper Analytic API
  slug: mrscraper-analytic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-analytic-api-openapi.yml
- filename: mrscraper-auth-api-openapi.yml
  format: yaml
  label: MrScraper Auth API
  slug: mrscraper-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-auth-api-openapi.yml
- filename: mrscraper-gateway-api-openapi.yml
  format: yaml
  label: MrScraper Gateway API
  slug: mrscraper-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-gateway-api-openapi.yml
- filename: mrscraper-jobs-api-openapi.yml
  format: yaml
  label: MrScraper Jobs API
  slug: mrscraper-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-jobs-api-openapi.yml
- filename: mrscraper-proxies-api-openapi.yml
  format: yaml
  label: MrScraper Proxies API
  slug: mrscraper-proxies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-proxies-api-openapi.yml
- filename: mrscraper-results-api-openapi.yml
  format: yaml
  label: MrScraper Results API
  slug: mrscraper-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-results-api-openapi.yml
- filename: mrscraper-storage-api-openapi.yml
  format: yaml
  label: MrScraper Storage API
  slug: mrscraper-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-storage-api-openapi.yml
- filename: mrscraper-tasks-api-openapi.yml
  format: yaml
  label: MrScraper Tasks API
  slug: mrscraper-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-tasks-api-openapi.yml
consequence_counts:
  read: 7
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mrscraper Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'MrScraper exposes 15 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MrScraper
provider_slug: mrscraper
slug: mrscraper-agentic-access
source_filename: mrscraper-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: generated\nsource: openapi/mrscraper-scraper-service-gateway-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 7\n    acting: 8\n  by_consequence:\n    read: 7\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: fetchPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: post\n  operationId: runScraper\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs\n  method: post\n  operationId: createJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}\n  method: put\n  operationId: updateJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage/{key}\n  method: get\n  operationId: getStoredResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscription-accounts\n  method: get\n  operationId: getSubscriptionAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks\n  method: get\n  operationId: listTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks\n  method: post\n  operationId: createTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/bulk\n  method: put\n  operationId: updateTasksBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/bulk\n  method: post\n  operationId: createTasksBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{id}\n  method: get\n  operationId: getTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /tasks/{id}\n  method: put\n  operationId: updateTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{id}/status\n  method: put\n  operationId: updateTaskStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/agentic-access/mrscraper-agentic-access.yml
summary_line: 15 operations · 8 acting
tags:
- Company
- Web Scraping
- Data Extraction
- Proxies
- AI Agents
- MCP
- Search
- Browser Automation
---

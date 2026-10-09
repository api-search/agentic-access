---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 19
api_specs:
- filename: ploid-account-api-openapi.yml
  format: yaml
  label: Ploid Account API
  slug: ploid-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-account-api-openapi.yml
- filename: ploid-discovery-api-openapi.yml
  format: yaml
  label: Ploid Discovery API
  slug: ploid-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-discovery-api-openapi.yml
- filename: ploid-enrichment-api-openapi.yml
  format: yaml
  label: Ploid Enrichment API
  slug: ploid-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-enrichment-api-openapi.yml
- filename: ploid-harness-api-openapi.yml
  format: yaml
  label: Ploid Harness API
  slug: ploid-harness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-harness-api-openapi.yml
- filename: ploid-monitors-api-openapi.yml
  format: yaml
  label: Ploid Monitors API
  slug: ploid-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-monitors-api-openapi.yml
- filename: ploid-people-api-openapi.yml
  format: yaml
  label: Ploid People API
  slug: ploid-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-people-api-openapi.yml
- filename: ploid-search-api-openapi.yml
  format: yaml
  label: Ploid Search API
  slug: ploid-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-search-api-openapi.yml
- filename: ploid-social-api-openapi.yml
  format: yaml
  label: Ploid Social API
  slug: ploid-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-social-api-openapi.yml
- filename: ploid-linked-in-api-openapi.yml
  format: yaml
  label: Ploid Linked In API
  slug: ploid-linked-in-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/openapi/ploid-linked-in-api-openapi.yml
consequence_counts:
  read: 19
  safety-critical: 2
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Ploid Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/account/key
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/monitors/{id}
operation_count: 31
overview: 'Ploid exposes 31 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 10 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ploid
provider_slug: ploid
slug: ploid-agentic-access
source_filename: ploid-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: generated\nsource: openapi/ploid-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 19\n    acting: 12\n  by_consequence:\n    read: 19\n    write: 10\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v1/openapi.json\n  method: get\n  operationId: getOpenApiDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/harness/context\n  method: post\n  operationId: getHarnessContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/harness/chat/completions\n  method: post\n  operationId: createHarnessChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/search\n  method: post\n  operationId: syncPeopleSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resolve\n  method: post\n  operationId: resolvePerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/person\n  method: post\n  operationId: getPerson\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/person/runs/{id}\n  method: get\n  operationId: getPersonRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/person/runs/{id}\n  method: delete\n  operationId: cancelPersonRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors/compile\n  method: post\n  operationId: compileMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors\n  method: post\n  operationId: createMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors\n  method: get\n  operationId: listMonitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors/{id}\n  method: get\n  operationId: getMonitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors/{id}\n  method: patch\n  operationId: updateMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors/{id}\n  method: delete\n  operationId: deleteMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/monitors/{id}/run\n  method: post\n  operationId: runMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors/{id}/runs\n  method: get\n  operationId: listMonitorRuns\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors/{id}/runs/{runId}\n  method: get\n  operationId: getMonitorRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors/{id}/items\n  method: get\n  operationId: listMonitorItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/socials\n  method: post\n  operationId: enrichSocialProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/linkedin/profile\n  method: get\n\
  \  operationId: getLinkedInProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/linkedin/search\n  method: post\n  operationId: searchLinkedInPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/linkedin/posts\n  method: get\n  operationId: listLinkedInPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/linkedin/profiles/comments\n  method: get\n  operationId: listLinkedInProfileComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/linkedin/companies/get\n  method: get\n  operationId: getLinkedInCompany\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/linkedin/companies/posts\n  method: get\n  operationId: listLinkedInCompanyPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrich\n  method: post\n  operationId: enrichPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/credits\n  method: get\n  operationId: getCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/usage\n  method: get\n  operationId: getAccountUsage\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/profile\n  method: get\n  operationId: getAccountProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/profile\n  method: patch\n  operationId: updateAccountProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/key\n  method: delete\n  operationId: revokeCurrentApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n  \
  \    proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ploid/refs/heads/main/agentic-access/ploid-agentic-access.yml
summary_line: 31 operations · 12 acting · 2 human-in-the-loop
tags:
- Company
- People Data
- People Search
- Contact Enrichment
- Sales Intelligence
- Recruiting
- LinkedIn
- MCP
- Agents
- Data Enrichment
---

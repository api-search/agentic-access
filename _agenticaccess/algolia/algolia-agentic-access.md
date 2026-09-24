---
acting_count: 168
action_class_counts:
  acting: 168
  connected: 174
api_specs:
- filename: algolia-search-api-openapi.yml
  format: yaml
  label: Algolia Search API
  slug: algolia-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-search-api-openapi.yml
- filename: algolia-insights-api-openapi.yml
  format: yaml
  label: Algolia Insights API
  slug: algolia-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-insights-api-openapi.yml
- filename: algolia-recommend-api-openapi.yml
  format: yaml
  label: Algolia Recommend API
  slug: algolia-recommend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-recommend-api-openapi.yml
- filename: algolia-analytics-api-openapi.yml
  format: yaml
  label: Algolia Analytics API
  slug: algolia-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-analytics-api-openapi.yml
- filename: algolia-abtesting-v3-api-openapi.yml
  format: yaml
  label: Algolia A/B Testing API
  slug: algolia-a-b-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-abtesting-v3-api-openapi.yml
- filename: algolia-personalization-api-openapi.yml
  format: yaml
  label: Algolia Personalization API
  slug: algolia-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-personalization-api-openapi.yml
- filename: algolia-advanced-personalization-api-openapi.yml
  format: yaml
  label: Algolia Advanced Personalization API
  slug: algolia-advanced-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-advanced-personalization-api-openapi.yml
- filename: algolia-crawler-api-openapi.yml
  format: yaml
  label: Algolia Crawler API
  slug: algolia-crawler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-crawler-api-openapi.yml
- filename: algolia-ingestion-api-openapi.yml
  format: yaml
  label: Algolia Ingestion API
  slug: algolia-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-ingestion-api-openapi.yml
- filename: algolia-query-suggestions-api-openapi.yml
  format: yaml
  label: Algolia Query Suggestions API
  slug: algolia-query-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-query-suggestions-api-openapi.yml
- filename: algolia-composition-api-openapi.yml
  format: yaml
  label: Algolia Composition API
  slug: algolia-composition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-composition-api-openapi.yml
- filename: algolia-agent-studio-api-openapi.yml
  format: yaml
  label: Algolia Agent Studio API
  slug: algolia-agent-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-agent-studio-api-openapi.yml
- filename: algolia-monitoring-api-openapi.yml
  format: yaml
  label: Algolia Monitoring API
  slug: algolia-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-monitoring-api-openapi.yml
- filename: algolia-ab-testing-api-openapi.yml
  format: yaml
  label: Algolia Ab Testing API
  slug: algolia-ab-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-ab-testing-api-openapi.yml
consequence_counts:
  physical: 41
  read: 174
  safety-critical: 4
  write: 123
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Algolia Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /1/tasks/{taskID}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /2/abtests/{id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /2/tasks/{taskID}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /3/abtests/{id}/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /1/events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /{path}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{path}
operation_count: 342
overview: 'Algolia exposes 342 API operations that an AI agent could call, of which 168 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 174 read, 123 write, 41 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Algolia
provider_slug: algolia
slug: algolia-agentic-access
source_filename: algolia-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/algolia-ab-testing-api-openapi.yml, openapi/algolia-abtesting-v3-api-openapi.yml,\n  openapi/algolia-advanced-personalization-api-openapi.yml, openapi/algolia-agent-studio-api-openapi.yml,\n  openapi/algolia-algoliasearch-api-openapi.yml, openapi/algolia-analytics-api-openapi.yml,\n  openapi/algolia-composition-api-openapi.yml, openapi/algolia-crawler-api-openapi.yml, openapi/algolia-ingestion-api-openapi.yml,\n  openapi/algolia-insights-api-openapi.yml, openapi/algolia-monitoring-api-openapi.yml, openapi/algolia-personalization-api-openapi.yml,\n  openapi/algolia-query-suggestions-api-openapi.yml, openapi/algolia-recommend-api-openapi.yml,\n  openapi/algolia-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\n\
  summary:\n  operations: 342\n  by_action_class:\n    connected: 174\n    acting: 168\n  by_consequence:\n    read: 174\n    physical: 41\n    write: 123\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /{path}\n  method: get\n  operationId: customGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{path}\n  method: post\n  operationId: customPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{path}\n  method: put\n  operationId: customPut\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{path}\n  method: delete\n  operationId: customDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2/abtests\n  method: post\n  operationId: addABTests\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2/abtests\n  method: get\n  operationId: listABTests\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/abtests/{id}\n  method: get\n  operationId: getABTest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/abtests/{id}\n  method: delete\n  operationId: deleteABTest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2/abtests/{id}/stop\n  method: post\n  operationId: stopABTest\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /2/abtests/estimate\n  method: post\n  operationId: estimateABTest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /setClientApiKey\n  method: get\n  operationId: setClientApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{path}\n  method: get\n  operationId: customGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{path}\n  method: post\n  operationId: customPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{path}\n  method: put\n  operationId: customPut\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{path}\n  method: delete\n  operationId: customDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /3/abtests\n  method: post\n  operationId: addABTests\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /3/abtests\n  method: get\n  operationId: listABTests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/abtests/{id}\n  method: get\n  operationId: getABTest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/abtests/{id}\n  method: delete\n  operationId: deleteABTest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /3/abtests/{id}/stop\n  method: post\n  operationId: stopABTest\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /3/abtests/estimate\n  method: post\n  operationId: estimateABTest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /3/abtests/{id}/timeseries\n  method: get\n  operationId: getTimeseries\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /setClientApiKey\n  method: get\n  operationId: setClientApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{path}\n  method: get\n  operationId: customGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{path}\n  method: post\n  operationId: customPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{path}\n  method: put\n  operationId: customPut\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{path}\n  method: delete\n  operationId: customDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2/config\n  method: get\n  operationId: getConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/config\n  method: put\n  operationId: putConfig\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2/users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/users/{userID}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/users/{userID}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /2/realtime/users/{userToken}\n  method: get\n  operationId: getRealtimeUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/realtime/users/{userToken}/compute\n  method: post\n  operationId: computeRealtimeUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /setClientApiKey\n  method: get\n  operationId: setClientApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /1/agents\n  method: post\n  operationId: createAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/agents/{agentId}\n  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/agents/{agentId}\n  method: patch\n  operationId: updateAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/agents/{agentId}\n  method: delete\n  operationId:\
  \ deleteAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/agents/{agentId}/allowed-domains\n  method: get\n  operationId: listAgentAllowedDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/agents/{agentId}/allowed-domains\n  method: post\n  operationId: createAgentAllowedDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/agents/{agentId}/allowed-domains/bulk\n  method: post\n  operationId: bulkCreateAllowedDomains\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/agents/{agentId}/allowed-domains/bulk\n  method: delete\n  operationId: bulkDeleteAllowedDomains\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/agents/{agentId}/allowed-domains/{domainId}\n  method: get\n  operationId: getAllowedDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/agents/{agentId}/allowed-domains/{domainId}\n  method: delete\n  operationId:\
  \ deleteAllowedDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/agents/{agentId}/cache\n  method: delete\n  operationId: invalidateAgentCache\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/agents/{agentId}/completions\n  method: post\n  operationId: createAgentCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /1/agents/{agentId}/conversations\n  method: get\n  operationId: listAgentConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/agents/{agentId}/conversations\n  method: delete\n  operationId: deleteAgentConversations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/agents/{agentId}/conversations/export\n  method: get\n  operationId: exportConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/agents/{agentId}/conversations/{conversationId}\n  method: get\n  operationId:\
  \ getConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/agents/{agentId}/conversations/{conversationId}\n  method: delete\n  operationId: deleteConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/agents/{agentId}/publish\n  method: post\n  operationId: publishAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/agents/{agentId}/unpublish\n  method: post\n  operationId: unpublishAgent\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/configuration\n  method: get\n  operationId: getConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/configuration\n  method: patch\n  operationId: updateConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/feedback\n  method: post\n  operationId: createFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/providers\n  method: get\n  operationId: listProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/providers\n  method: post\n  operationId: createProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/providers/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/providers/{providerId}\n\
  \  method: get\n  operationId: getProvider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/providers/{providerId}\n  method: patch\n  operationId: updateProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/providers/{providerId}\n  method: delete\n  operationId: deleteProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/providers/{providerId}/models\n  method: get\n  operationId: listProviderModels\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/secret-keys\n  method: get\n  operationId: listSecretKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/secret-keys\n  method: post\n  operationId: createSecretKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/secret-keys/{secretKeyId}\n  method: get\n  operationId: getSecretKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/secret-keys/{secretKeyId}\n  method: patch\n  operationId:\
  \ updateSecretKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/secret-keys/{secretKeyId}\n  method: delete\n  operationId: deleteSecretKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/user-data/{userToken}\n  method: get\n  operationId: getUserData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/user-data/{userToken}\n  method: delete\n  operationId: deleteUserData\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{path}\n  method: get\n  operationId: customGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{path}\n  method: post\n  operationId: customPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{path}\n  method: put\n  operationId: customPut\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{path}\n  method: delete\n  operationId: customDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /setClientApiKey\n  method: get\n  operationId: setClientApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{path}\n  method: post\n  operationId: customPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1/indexes/*/queries\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1/indexes/*/recommendations\n  method: post\n  operationId: getRecommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{path}\n  method: get\n  operationId: customGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{path}\n  method: post\n  operationId: customPost\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{path}\n  method: put\n  operationId: customPut\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{path}\n  method: delete\n  operationId: customDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /2/searches\n  method: get\n  operationId: getTopSearches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/searches/count\n  method: get\n  operationId: getSearchesCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/searches/noResults\n  method: get\n  operationId: getSearchesNoResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/searches/noClicks\n  method: get\n  operationId: getSearchesNoClicks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/searches/noResultRate\n  method: get\n  operationId:\
  \ getNoResultsRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/searches/noClickRate\n  method: get\n  operationId: getNoClickRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/hits\n  method: get\n  operationId: getTopHits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/users/count\n  method: get\n  operationId: getUsersCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/filters\n  method: get\n  operationId: getTopFilterAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /2/filters/{attribute}\n  method: get\n  operationId: getTopFilterForAttribute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/filters/noResults\n  method: get\n  operationId: getTopFiltersNoResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/countries\n  method: get\n  operationId: getTopCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/clicks/averageClickPosition\n  method: get\n  operationId: getAverageClickPosition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/clicks/positions\n  method: get\n  operationId:\
  \ getClickPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/clicks/clickThroughRate\n  method: get\n  operationId: getClickThroughRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/conversions/conversionRate\n  method: get\n  operationId: getConversionRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/conversions/addToCartRate\n  method: get\n  operationId: getAddToCartRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/conversions/purchaseRate\n  method: get\n  operationId: getPurchaseRate\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/conversions/revenue\n  method: get\n  operationId: getRevenue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/patterns/fields\n  method: get\n  operationId: getPatternsFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/patterns/timeseries\n  method: post\n  operationId: queryPatternsTimeseries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/patterns/scalar\n\
  \  method: post\n  operationId: queryPatternsScalar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/patterns/table\n  method: post\n  operationId: queryPatternsTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3/patterns/distribution\n  method: post\n  operationId: queryPatternsDistribution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /setClientApiKey\n  method: get\n  operationId: setClientApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{path}\n  method: get\n  operationId: customGet\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{path}\n  method: post\n  operationId: customPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{path}\n  method: put\n  operationId: customPut\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (95 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/agentic-access/algolia-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/agentic-access/algolia-agentic-access.yml
summary_line: 342 operations · 168 acting · 4 human-in-the-loop
tags:
- Search
- Discovery
- Recommendations
- Personalization
- Analytics
- E-Commerce
---

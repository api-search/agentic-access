---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 19
api_specs:
- filename: keen-event-collection-api-openapi.yml
  format: yaml
  label: Keen Event Collection API
  slug: event-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keen/refs/heads/main/openapi/keen-event-collection-api-openapi.yml
- filename: keen-query-api-openapi.yml
  format: yaml
  label: Keen Query API
  slug: query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keen/refs/heads/main/openapi/keen-query-api-openapi.yml
- filename: keen-cached-queries-api-openapi.yml
  format: yaml
  label: Keen Cached Queries API
  slug: cached-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keen/refs/heads/main/openapi/keen-cached-queries-api-openapi.yml
- filename: keen-saved-queries-api-openapi.yml
  format: yaml
  label: Keen Saved Queries API
  slug: saved-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keen/refs/heads/main/openapi/keen-saved-queries-api-openapi.yml
- filename: keen-data-extraction-api-openapi.yml
  format: yaml
  label: Keen Data Extraction API
  slug: data-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keen/refs/heads/main/openapi/keen-data-extraction-api-openapi.yml
consequence_counts:
  read: 19
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Keen Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Keen exposes 27 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Keen
provider_slug: keen
slug: keen-agentic-access
source_filename: keen-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/keen-cached-queries-api-openapi.yml, openapi/keen-data-extraction-api-openapi.yml,\n  openapi/keen-event-collection-api-openapi.yml, openapi/keen-query-api-openapi.yml, openapi/keen-saved-queries-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 19\n    acting: 8\n  by_consequence:\n    read: 19\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /projects/{projectId}/queries/cached\n  method: get\n  operationId: listCachedQueries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/queries/cached/{queryName}\n\
  \  method: get\n  operationId: getCachedQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/queries/cached/{queryName}\n  method: put\n  operationId: createOrUpdateCachedQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/queries/cached/{queryName}\n  method: delete\n  operationId: deleteCachedQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/queries/cached/{queryName}/result\n\
  \  method: get\n  operationId: getCachedQueryResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/queries/extraction\n  method: get\n  operationId: extractEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/events/{eventCollection}\n  method: post\n  operationId: recordEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/events/{eventCollection}\n  method: get\n  operationId: inspectCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/events\n  method: post\n  operationId: recordEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/events\n  method: get\n  operationId: listCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/events/{eventCollection}/properties/{propertyName}\n  method: get\n  operationId: inspectProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/queries/count\n  method: get\n  operationId:\
  \ queryCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/queries/count_unique\n  method: get\n  operationId: queryCountUnique\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/queries/sum\n  method: get\n  operationId: querySum\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/queries/average\n  method: get\n  operationId: queryAverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/queries/minimum\n  method: get\n  operationId: queryMinimum\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/queries/maximum\n  method: get\n  operationId: queryMaximum\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/queries/median\n  method: get\n  operationId: queryMedian\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/queries/percentile\n  method: get\n  operationId: queryPercentile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/queries/select_unique\n  method: get\n  operationId: querySelectUnique\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/queries/funnel\n  method: post\n  operationId: queryFunnel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/queries/multi_analysis\n  method: post\n  operationId: queryMultiAnalysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/queries/saved\n  method: get\n  operationId: listSavedQueries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/queries/saved/{queryName}\n  method: get\n  operationId: getSavedQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/queries/saved/{queryName}\n  method: put\n  operationId: createOrUpdateSavedQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/queries/saved/{queryName}\n  method: delete\n  operationId: deleteSavedQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/queries/saved/{queryName}/result\n  method: get\n  operationId: runSavedQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keen/refs/heads/main/agentic-access/keen-agentic-access.yml
summary_line: 27 operations · 8 acting
tags:
- Analytics
- Custom Events
- Data Collection
- Embedded Analytics
- Event Analytics
---

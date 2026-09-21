---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 26
api_specs:
- filename: perigon-ai-advanced-search-api-openapi.yml
  format: yaml
  label: Perigon AI & Advanced Search API
  slug: perigon-ai-advanced-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-ai-advanced-search-api-openapi.yml
- filename: perigon-contact-points-api-openapi.yml
  format: yaml
  label: Perigon Contact Points API
  slug: perigon-contact-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-contact-points-api-openapi.yml
- filename: perigon-monitors-api-openapi.yml
  format: yaml
  label: Perigon Monitors API
  slug: perigon-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-monitors-api-openapi.yml
- filename: perigon-news-stories-api-openapi.yml
  format: yaml
  label: Perigon News & Stories API
  slug: perigon-news-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-news-stories-api-openapi.yml
- filename: perigon-source-groups-api-openapi.yml
  format: yaml
  label: Perigon Source Groups API
  slug: perigon-source-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-source-groups-api-openapi.yml
- filename: perigon-supplemental-endpoints-api-openapi.yml
  format: yaml
  label: Perigon Supplemental Endpoints API
  slug: perigon-supplemental-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-supplemental-endpoints-api-openapi.yml
- filename: perigon-utilities-api-openapi.yml
  format: yaml
  label: Perigon Utilities API
  slug: perigon-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-utilities-api-openapi.yml
- filename: perigon-watchlists-api-openapi.yml
  format: yaml
  label: Perigon Watchlists API
  slug: perigon-watchlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-watchlists-api-openapi.yml
- filename: perigon-wikipedia-api-openapi.yml
  format: yaml
  label: Perigon Wikipedia API
  slug: perigon-wikipedia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/openapi/perigon-wikipedia-api-openapi.yml
consequence_counts:
  read: 26
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Perigon Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 45
overview: 'Perigon exposes 45 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read and 19 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Perigon
provider_slug: perigon
slug: perigon-agentic-access
source_filename: perigon-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: generated\nsource: openapi/perigon-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 45\n  by_action_class:\n    connected: 26\n    acting: 19\n  by_consequence:\n    read: 26\n    write: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/api/contactPoints\n  method: get\n  operationId: list-contact-points\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/contactPoints\n  method: post\n  operationId: create-contact-point\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/contactPoints/{uuid}\n  method: get\n  operationId: get-contact-point\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/contactPoints/{uuid}\n  method: delete\n  operationId: delete-contact-point\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/contactPoints/{uuid}\n  method: patch\n  operationId: update-contact-point\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/monitors\n  method: get\n  operationId: list-monitors-api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/monitors\n  method: post\n  operationId: create-monitor-api\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/monitors/{uuid}\n  method: get\n  operationId: get-monitor-api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/monitors/{uuid}\n  method: delete\n  operationId: archive-monitor-api\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/monitors/{uuid}\n  method: patch\n  operationId: update-monitor-api\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/monitors/{uuid}/activate\n  method: post\n  operationId: activate-monitor-api\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/monitors/{uuid}/events\n\
  \  method: get\n  operationId: list-monitor-events-api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/monitors/{uuid}/newsletters\n  method: get\n  operationId: list-monitor-newsletters-api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/monitors/{uuid}/pause\n  method: post\n  operationId: pause-monitor-api\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/monitors/{uuid}/summary\n  method: get\n  operationId: list-monitor-summaries-api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/sourceGroups\n  method: get\n  operationId: list-source-groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/sourceGroups\n  method: post\n  operationId: create-source-group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/sourceGroups/resolve\n  method: get\n  operationId: resolve-source-groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/sourceGroups/{id}\n  method: get\n  operationId: get-source-group\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/sourceGroups/{id}\n  method: delete\n  operationId: delete-source-group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/sourceGroups/{id}\n  method: patch\n  operationId: update-source-group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/watchlists\n  method: get\n  operationId: list-watchlists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/watchlists\n  method: post\n  operationId: create-watchlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/watchlists/resolve\n  method: get\n  operationId: resolve-watchlists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/watchlists/{id}\n  method: get\n  operationId: get-watchlist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/watchlists/{id}\n  method: delete\n  operationId: delete-watchlist\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/watchlists/{id}\n  method: patch\n  operationId: update-watchlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/articles/all\n  method: get\n  operationId: search-articles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/articles/refresh/jobs\n  method: post\n  operationId: submit-article-refresh-job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/articles/refresh/jobs/{id}\n  method: get\n  operationId: get-article-refresh-job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/articles/refresh/peek\n  method: post\n  operationId: peek-article-refresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/all\n  method: get\n  operationId: search-companies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/journalists/all\n  method: get\n  operationId: search-journalists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/journalists/{id}\n  method: get\n  operationId: get-journalist-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/limits\n  method: get\n  operationId: get-limits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/people/all\n  method: get\n  operationId: search-people\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sources/all\n  method: get\n  operationId: search-sources\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stories/all\n  method: get\n  operationId: search-stories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stories/history\n  method: get\n  operationId: get-story-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stories/stats\n  method: get\n  operationId: get-story-counts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/summarize\n  method: post\n  operationId: search-summarizer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/topics/all\n  method: get\n  operationId: search-topics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vector/news/all\n  method: post\n  operationId: vector-search-articles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vector/wikipedia/all\n  method: post\n  operationId: vector-search-wikipedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /v1/wikipedia/all\n  method: get\n  operationId: search-wikipedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perigon/refs/heads/main/agentic-access/perigon-agentic-access.yml
summary_line: 45 operations · 19 acting
tags:
- Company
- News
- Media Monitoring
- Search
- Artificial Intelligence
- Data
- MCP
- Webhook
---

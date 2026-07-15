---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 17
api_specs:
- filename: semantic-scholar-academic-graph-openapi.yml
  format: yaml
  label: Semantic Scholar Academic Graph API
  slug: semantic-scholar-academic-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semantic-scholar/refs/heads/main/openapi/semantic-scholar-academic-graph-openapi.yml
- filename: semantic-scholar-recommendations-openapi.yml
  format: yaml
  label: Semantic Scholar Recommendations API
  slug: semantic-scholar-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semantic-scholar/refs/heads/main/openapi/semantic-scholar-recommendations-openapi.yml
- filename: semantic-scholar-datasets-openapi.yml
  format: yaml
  label: Semantic Scholar Datasets API
  slug: semantic-scholar-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semantic-scholar/refs/heads/main/openapi/semantic-scholar-datasets-openapi.yml
consequence_counts:
  read: 17
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Semantic Scholar Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Semantic Scholar exposes 20 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Semantic Scholar
provider_slug: semantic-scholar
slug: semantic-scholar-agentic-access
source_filename: semantic-scholar-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/semantic-scholar-academic-graph-openapi.yml, openapi/semantic-scholar-datasets-openapi.yml,\n  openapi/semantic-scholar-recommendations-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 3\n    connected: 17\n  by_consequence:\n    write: 3\n    read: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /author/batch\n  method: post\n  operationId: post_graph_get_authors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /author/search\n  method: get\n  operationId: get_graph_get_author_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /author/{author_id}\n  method: get\n  operationId: get_graph_get_author\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /author/{author_id}/papers\n  method: get\n  operationId: get_graph_get_author_papers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paper/autocomplete\n  method: get\n  operationId: get_graph_get_paper_autocomplete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paper/batch\n  method: post\n  operationId:\
  \ post_graph_get_papers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paper/search\n  method: get\n  operationId: get_graph_paper_relevance_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paper/search/bulk\n  method: get\n  operationId: get_graph_paper_bulk_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paper/search/match\n  method: get\n  operationId: get_graph_paper_title_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /paper/{paper_id}\n  method: get\n  operationId: get_graph_get_paper\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paper/{paper_id}/authors\n  method: get\n  operationId: get_graph_get_paper_authors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paper/{paper_id}/citations\n  method: get\n  operationId: get_graph_get_paper_citations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paper/{paper_id}/references\n  method: get\n  operationId: get_graph_get_paper_references\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /snippet/search\n  method: get\n  operationId:\
  \ get_snippet_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /diffs/{start_release_id}/to/{end_release_id}/{dataset_name}\n  method: get\n  operationId: get_diff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /release/\n  method: get\n  operationId: get_releases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /release/{release_id}\n  method: get\n  operationId: get_release\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /release/{release_id}/dataset/{dataset_name}\n  method: get\n  operationId: get_dataset\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /papers/\n  method: post\n  operationId: post_papers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /papers/forpaper/{paper_id}\n  method: get\n  operationId: get_papers_for_paper\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/semantic-scholar/refs/heads/main/agentic-access/semantic-scholar-agentic-access.yml
summary_line: 20 operations · 3 acting
tags:
- Academic
- Research
- Papers
- Citations
- Authors
- Scientific Literature
- AI
- Recommendations
---

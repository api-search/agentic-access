---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: dtu-data.yaml
  format: yaml
  label: DTU Data (Figshare API)
  slug: data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dtu/refs/heads/main/openapi/dtu-data.yaml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dtu Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Technical University of Denmark exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Technical University of Denmark
provider_slug: dtu
slug: dtu-agentic-access
source_filename: dtu-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/dtu-data.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /articles\n  method: get\n  operationId: articles_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{article_id}\n  method: get\n  operationId: article_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{article_id}/files\n  method: get\n  operationId: article_files\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{article_id}/files/{file_id}\n  method: get\n  operationId: article_file_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{article_id}/versions\n  method: get\n  operationId: article_versions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{article_id}/versions/{version_id}\n  method: get\n  operationId: article_version_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /institutions/{institution_string_id}/articles/filter-by\n  method: get\n  operationId: institution_articles\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dtu/refs/heads/main/agentic-access/dtu-agentic-access.yml
summary_line: 7 operations
tags:
- Education
- Higher Education
- University
- Research Data
- Open Data
- Denmark
- Europe
---
